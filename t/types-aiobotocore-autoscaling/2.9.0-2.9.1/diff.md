# Comparing `tmp/types-aiobotocore-autoscaling-2.9.0.tar.gz` & `tmp/types-aiobotocore-autoscaling-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-2.9.0.tar", last modified: Wed Dec 13 19:58:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-2.9.1.tar", last modified: Thu Jan 18 01:20:06 2024, max compression
```

## Comparing `types-aiobotocore-autoscaling-2.9.0.tar` & `types-aiobotocore-autoscaling-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:38.726061 types-aiobotocore-autoscaling-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2023-12-13 19:58:38.726061 types-aiobotocore-autoscaling-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:38.726061 types-aiobotocore-autoscaling-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:38.726061 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55954 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    55950 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14955 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    68348 2023-12-13 19:41:29.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    68347 2023-12-13 19:41:28.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:27.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:38.726061 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2023-12-13 19:58:38.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 19:58:38.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:38.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:38.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:38.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:58:38.000000 types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.493501 types-aiobotocore-autoscaling-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-01-18 01:20:06.493501 types-aiobotocore-autoscaling-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:06.493501 types-aiobotocore-autoscaling-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.489501 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55976 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55973 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-01-18 01:03:26.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-01-18 01:03:26.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68347 2024-01-18 01:03:27.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68347 2024-01-18 01:03:27.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:25.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:06.493501 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:06.000000 types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/LICENSE` & `types-aiobotocore-autoscaling-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-autoscaling-2.9.0/PKG-INFO` & `types-aiobotocore-autoscaling-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AutoScaling 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AutoScaling 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
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
 
 <a id="types-aiobotocore-autoscaling"></a>
 
 # types-aiobotocore-autoscaling
 
 [![PyPI - types-aiobotocore-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScaling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[aiobotocore.AutoScaling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [types-aiobotocore-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/README.md` & `types-aiobotocore-autoscaling-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScaling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[aiobotocore.AutoScaling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [types-aiobotocore-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/setup.py` & `types-aiobotocore-autoscaling-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AutoScaling 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AutoScaling 2.9.1 service generated with"
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
     keywords="aiobotocore autoscaling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_autoscaling": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/__init__.py` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
     DescribeWarmPoolPaginator,
 )
 
 Client = AutoScalingClient
 
-
 __all__ = (
     "AutoScalingClient",
     "Client",
     "DescribeAutoScalingGroupsPaginator",
     "DescribeAutoScalingInstancesPaginator",
     "DescribeLaunchConfigurationsPaginator",
     "DescribeLoadBalancerTargetGroupsPaginator",
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/__init__.pyi` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/__main__.py` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AutoScaling 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AutoScaling 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
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

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/client.py` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AutoScalingClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -187,15 +186,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#batch_delete_scheduled_action)
         """
 
     async def batch_put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
-        ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef]
+        ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef],
     ) -> BatchPutScheduledUpdateGroupActionAnswerTypeDef:
         """
         Creates or updates one or more scheduled scaling actions for an Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_put_scheduled_update_group_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#batch_put_scheduled_update_group_action)
@@ -230,15 +229,15 @@
     async def complete_lifecycle_action(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionResult: str,
         LifecycleActionToken: str = ...,
-        InstanceId: str = ...
+        InstanceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Completes the lifecycle action for the specified token or instance with the
         specified
         result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.complete_lifecycle_action)
@@ -271,15 +270,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         ServiceLinkedRoleARN: str = ...,
         MaxInstanceLifetime: int = ...,
         Context: str = ...,
         DesiredCapacityType: str = ...,
         DefaultInstanceWarmup: int = ...,
         TrafficSources: Sequence[TrafficSourceIdentifierTypeDef] = ...,
-        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...
+        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         **We strongly recommend using a launch template when calling this operation to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Creates
         an Auto Scaling group with the specified name and
         attributes.
 
@@ -304,15 +303,15 @@
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         InstanceMonitoring: InstanceMonitoringTypeDef = ...,
         SpotPrice: str = ...,
         IamInstanceProfile: str = ...,
         EbsOptimized: bool = ...,
         AssociatePublicIpAddress: bool = ...,
         PlacementTenancy: str = ...,
-        MetadataOptions: InstanceMetadataOptionsTypeDef = ...
+        MetadataOptions: InstanceMetadataOptionsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a launch configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#create_launch_configuration)
         """
@@ -424,15 +423,15 @@
 
     async def describe_auto_scaling_groups(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> AutoScalingGroupsTypeTypeDef:
         """
         Gets information about the Auto Scaling groups in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_auto_scaling_groups)
         """
@@ -459,30 +458,30 @@
 
     async def describe_instance_refreshes(
         self,
         *,
         AutoScalingGroupName: str,
         InstanceRefreshIds: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeInstanceRefreshesAnswerTypeDef:
         """
         Gets information about the instance refreshes for the specified Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_instance_refreshes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_instance_refreshes)
         """
 
     async def describe_launch_configurations(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> LaunchConfigurationsTypeTypeDef:
         """
         Gets information about the launch configurations in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_launch_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_launch_configurations)
         """
@@ -534,15 +533,15 @@
         """
 
     async def describe_notification_configurations(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeNotificationConfigurationsAnswerTypeDef:
         """
         Gets information about the Amazon SNS notifications that are configured for one
         or more Auto Scaling
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_notification_configurations)
@@ -552,15 +551,15 @@
     async def describe_policies(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PoliciesTypeTypeDef:
         """
         Gets information about the scaling policies in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_policies)
         """
@@ -568,15 +567,15 @@
     async def describe_scaling_activities(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ActivitiesTypeTypeDef:
         """
         Gets information about the scaling activities in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scaling_activities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_scaling_activities)
         """
@@ -595,15 +594,15 @@
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> ScheduledActionsTypeTypeDef:
         """
         Gets information about the scheduled actions that haven't run or that have not
         reached their end
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scheduled_actions)
@@ -632,15 +631,15 @@
 
     async def describe_traffic_sources(
         self,
         *,
         AutoScalingGroupName: str,
         TrafficSourceType: str = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeTrafficSourcesResponseTypeDef:
         """
         Gets information about the traffic sources for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_traffic_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_traffic_sources)
         """
@@ -656,15 +655,15 @@
         """
 
     async def detach_instances(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
-        InstanceIds: Sequence[str] = ...
+        InstanceIds: Sequence[str] = ...,
     ) -> DetachInstancesAnswerTypeDef:
         """
         Removes one or more instances from the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#detach_instances)
         """
@@ -720,15 +719,15 @@
         """
 
     async def enter_standby(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
-        InstanceIds: Sequence[str] = ...
+        InstanceIds: Sequence[str] = ...,
     ) -> EnterStandbyAnswerTypeDef:
         """
         Moves the specified instances into the standby state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.enter_standby)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#enter_standby)
         """
@@ -736,15 +735,15 @@
     async def execute_policy(
         self,
         *,
         PolicyName: str,
         AutoScalingGroupName: str = ...,
         HonorCooldown: bool = ...,
         MetricValue: float = ...,
-        BreachThreshold: float = ...
+        BreachThreshold: float = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Executes the specified policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.execute_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#execute_policy)
         """
@@ -775,15 +774,15 @@
 
     async def get_predictive_scaling_forecast(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
         StartTime: TimestampTypeDef,
-        EndTime: TimestampTypeDef
+        EndTime: TimestampTypeDef,
     ) -> GetPredictiveScalingForecastAnswerTypeDef:
         """
         Retrieves the forecast data for a predictive scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_predictive_scaling_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_predictive_scaling_forecast)
         """
@@ -794,15 +793,15 @@
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleTransition: str = ...,
         RoleARN: str = ...,
         NotificationTargetARN: str = ...,
         NotificationMetadata: str = ...,
         HeartbeatTimeout: int = ...,
-        DefaultResult: str = ...
+        DefaultResult: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a lifecycle hook for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_lifecycle_hook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_lifecycle_hook)
         """
@@ -831,15 +830,15 @@
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
         TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...,
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scaling_policy)
         """
@@ -852,15 +851,15 @@
         Time: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Recurrence: str = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
-        TimeZone: str = ...
+        TimeZone: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a scheduled scaling action for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scheduled_update_group_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scheduled_update_group_action)
         """
@@ -868,30 +867,30 @@
     async def put_warm_pool(
         self,
         *,
         AutoScalingGroupName: str,
         MaxGroupPreparedCapacity: int = ...,
         MinSize: int = ...,
         PoolState: WarmPoolStateType = ...,
-        InstanceReusePolicy: InstanceReusePolicyTypeDef = ...
+        InstanceReusePolicy: InstanceReusePolicyTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a warm pool for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_warm_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_warm_pool)
         """
 
     async def record_lifecycle_action_heartbeat(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionToken: str = ...,
-        InstanceId: str = ...
+        InstanceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Records a heartbeat for the lifecycle action associated with the specified
         token or
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.record_lifecycle_action_heartbeat)
@@ -954,15 +953,15 @@
 
     async def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
         DesiredConfiguration: DesiredConfigurationTypeDef = ...,
-        Preferences: RefreshPreferencesTypeDef = ...
+        Preferences: RefreshPreferencesTypeDef = ...,
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#start_instance_refresh)
         """
@@ -1009,15 +1008,15 @@
         NewInstancesProtectedFromScaleIn: bool = ...,
         ServiceLinkedRoleARN: str = ...,
         MaxInstanceLifetime: int = ...,
         CapacityRebalance: bool = ...,
         Context: str = ...,
         DesiredCapacityType: str = ...,
         DefaultInstanceWarmup: int = ...,
-        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...
+        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         **We strongly recommend that all Auto Scaling groups use launch templates to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Updates
         the configuration for the specified Auto Scaling
         group.
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/client.pyi` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#batch_delete_scheduled_action)
         """
 
     async def batch_put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
-        ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef]
+        ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef],
     ) -> BatchPutScheduledUpdateGroupActionAnswerTypeDef:
         """
         Creates or updates one or more scheduled scaling actions for an Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_put_scheduled_update_group_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#batch_put_scheduled_update_group_action)
@@ -226,15 +226,15 @@
     async def complete_lifecycle_action(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionResult: str,
         LifecycleActionToken: str = ...,
-        InstanceId: str = ...
+        InstanceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Completes the lifecycle action for the specified token or instance with the
         specified
         result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.complete_lifecycle_action)
@@ -267,15 +267,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         ServiceLinkedRoleARN: str = ...,
         MaxInstanceLifetime: int = ...,
         Context: str = ...,
         DesiredCapacityType: str = ...,
         DefaultInstanceWarmup: int = ...,
         TrafficSources: Sequence[TrafficSourceIdentifierTypeDef] = ...,
-        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...
+        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         **We strongly recommend using a launch template when calling this operation to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Creates
         an Auto Scaling group with the specified name and
         attributes.
 
@@ -300,15 +300,15 @@
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         InstanceMonitoring: InstanceMonitoringTypeDef = ...,
         SpotPrice: str = ...,
         IamInstanceProfile: str = ...,
         EbsOptimized: bool = ...,
         AssociatePublicIpAddress: bool = ...,
         PlacementTenancy: str = ...,
-        MetadataOptions: InstanceMetadataOptionsTypeDef = ...
+        MetadataOptions: InstanceMetadataOptionsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a launch configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#create_launch_configuration)
         """
@@ -420,15 +420,15 @@
 
     async def describe_auto_scaling_groups(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxRecords: int = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> AutoScalingGroupsTypeTypeDef:
         """
         Gets information about the Auto Scaling groups in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_auto_scaling_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_auto_scaling_groups)
         """
@@ -455,30 +455,30 @@
 
     async def describe_instance_refreshes(
         self,
         *,
         AutoScalingGroupName: str,
         InstanceRefreshIds: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeInstanceRefreshesAnswerTypeDef:
         """
         Gets information about the instance refreshes for the specified Auto Scaling
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_instance_refreshes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_instance_refreshes)
         """
 
     async def describe_launch_configurations(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> LaunchConfigurationsTypeTypeDef:
         """
         Gets information about the launch configurations in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_launch_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_launch_configurations)
         """
@@ -530,15 +530,15 @@
         """
 
     async def describe_notification_configurations(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeNotificationConfigurationsAnswerTypeDef:
         """
         Gets information about the Amazon SNS notifications that are configured for one
         or more Auto Scaling
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_notification_configurations)
@@ -548,15 +548,15 @@
     async def describe_policies(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PoliciesTypeTypeDef:
         """
         Gets information about the scaling policies in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_policies)
         """
@@ -564,15 +564,15 @@
     async def describe_scaling_activities(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
         MaxRecords: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ActivitiesTypeTypeDef:
         """
         Gets information about the scaling activities in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scaling_activities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_scaling_activities)
         """
@@ -591,15 +591,15 @@
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> ScheduledActionsTypeTypeDef:
         """
         Gets information about the scheduled actions that haven't run or that have not
         reached their end
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_scheduled_actions)
@@ -628,15 +628,15 @@
 
     async def describe_traffic_sources(
         self,
         *,
         AutoScalingGroupName: str,
         TrafficSourceType: str = ...,
         NextToken: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeTrafficSourcesResponseTypeDef:
         """
         Gets information about the traffic sources for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_traffic_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_traffic_sources)
         """
@@ -652,15 +652,15 @@
         """
 
     async def detach_instances(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
-        InstanceIds: Sequence[str] = ...
+        InstanceIds: Sequence[str] = ...,
     ) -> DetachInstancesAnswerTypeDef:
         """
         Removes one or more instances from the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#detach_instances)
         """
@@ -716,15 +716,15 @@
         """
 
     async def enter_standby(
         self,
         *,
         AutoScalingGroupName: str,
         ShouldDecrementDesiredCapacity: bool,
-        InstanceIds: Sequence[str] = ...
+        InstanceIds: Sequence[str] = ...,
     ) -> EnterStandbyAnswerTypeDef:
         """
         Moves the specified instances into the standby state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.enter_standby)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#enter_standby)
         """
@@ -732,15 +732,15 @@
     async def execute_policy(
         self,
         *,
         PolicyName: str,
         AutoScalingGroupName: str = ...,
         HonorCooldown: bool = ...,
         MetricValue: float = ...,
-        BreachThreshold: float = ...
+        BreachThreshold: float = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Executes the specified policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.execute_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#execute_policy)
         """
@@ -771,15 +771,15 @@
 
     async def get_predictive_scaling_forecast(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
         StartTime: TimestampTypeDef,
-        EndTime: TimestampTypeDef
+        EndTime: TimestampTypeDef,
     ) -> GetPredictiveScalingForecastAnswerTypeDef:
         """
         Retrieves the forecast data for a predictive scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_predictive_scaling_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_predictive_scaling_forecast)
         """
@@ -790,15 +790,15 @@
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleTransition: str = ...,
         RoleARN: str = ...,
         NotificationTargetARN: str = ...,
         NotificationMetadata: str = ...,
         HeartbeatTimeout: int = ...,
-        DefaultResult: str = ...
+        DefaultResult: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a lifecycle hook for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_lifecycle_hook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_lifecycle_hook)
         """
@@ -827,15 +827,15 @@
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
         TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...,
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scaling_policy)
         """
@@ -848,15 +848,15 @@
         Time: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Recurrence: str = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
-        TimeZone: str = ...
+        TimeZone: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a scheduled scaling action for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scheduled_update_group_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scheduled_update_group_action)
         """
@@ -864,30 +864,30 @@
     async def put_warm_pool(
         self,
         *,
         AutoScalingGroupName: str,
         MaxGroupPreparedCapacity: int = ...,
         MinSize: int = ...,
         PoolState: WarmPoolStateType = ...,
-        InstanceReusePolicy: InstanceReusePolicyTypeDef = ...
+        InstanceReusePolicy: InstanceReusePolicyTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a warm pool for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_warm_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_warm_pool)
         """
 
     async def record_lifecycle_action_heartbeat(
         self,
         *,
         LifecycleHookName: str,
         AutoScalingGroupName: str,
         LifecycleActionToken: str = ...,
-        InstanceId: str = ...
+        InstanceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Records a heartbeat for the lifecycle action associated with the specified
         token or
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.record_lifecycle_action_heartbeat)
@@ -950,15 +950,15 @@
 
     async def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
         DesiredConfiguration: DesiredConfigurationTypeDef = ...,
-        Preferences: RefreshPreferencesTypeDef = ...
+        Preferences: RefreshPreferencesTypeDef = ...,
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#start_instance_refresh)
         """
@@ -1005,15 +1005,15 @@
         NewInstancesProtectedFromScaleIn: bool = ...,
         ServiceLinkedRoleARN: str = ...,
         MaxInstanceLifetime: int = ...,
         CapacityRebalance: bool = ...,
         Context: str = ...,
         DesiredCapacityType: str = ...,
         DefaultInstanceWarmup: int = ...,
-        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...
+        InstanceMaintenancePolicy: InstanceMaintenancePolicyTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         **We strongly recommend that all Auto Scaling groups use launch templates to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Updates
         the configuration for the specified Auto Scaling
         group.
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/literals.py` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/literals.py`

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
     "AcceleratorManufacturerType",
     "AcceleratorNameType",
     "AcceleratorTypeType",
     "BareMetalType",
     "BurstablePerformanceType",
     "CpuManufacturerType",
@@ -61,15 +60,14 @@
     "AutoScalingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceleratorManufacturerType = Literal["amazon-web-services", "amd", "nvidia", "xilinx"]
 AcceleratorNameType = Literal["a100", "k80", "m60", "radeon-pro-v520", "t4", "v100", "vu9p"]
 AcceleratorTypeType = Literal["fpga", "gpu", "inference"]
 BareMetalType = Literal["excluded", "included", "required"]
 BurstablePerformanceType = Literal["excluded", "included", "required"]
 CpuManufacturerType = Literal["amazon-web-services", "amd", "intel"]
 DescribeAutoScalingGroupsPaginatorName = Literal["describe_auto_scaling_groups"]
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/literals.pyi` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/paginator.py` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
     "DescribeWarmPoolPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -95,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[AutoScalingGroupsTypePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
 
@@ -128,15 +127,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
 
@@ -176,15 +175,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
 
@@ -196,15 +195,15 @@
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describepoliciespaginator)
         """
 
 
@@ -216,15 +215,15 @@
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 
@@ -237,15 +236,15 @@
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -255,15 +254,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/paginator.pyi` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[AutoScalingGroupsTypePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
 class DescribeAutoScalingInstancesPaginator(AioPaginator):
@@ -123,15 +123,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
 class DescribeLoadBalancerTargetGroupsPaginator(AioPaginator):
@@ -168,15 +168,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
 class DescribePoliciesPaginator(AioPaginator):
@@ -187,15 +187,15 @@
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describepoliciespaginator)
         """
 
 class DescribeScalingActivitiesPaginator(AioPaginator):
@@ -206,15 +206,15 @@
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 class DescribeScheduledActionsPaginator(AioPaginator):
@@ -226,15 +226,15 @@
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
@@ -243,15 +243,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
         """
 
 class DescribeWarmPoolPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/type_defs.py` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmSpecificationTypeDef",
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling/type_defs.pyi` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AutoScaling 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AutoScaling 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
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
 
 <a id="types-aiobotocore-autoscaling"></a>
 
 # types-aiobotocore-autoscaling
 
 [![PyPI - types-aiobotocore-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScaling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[aiobotocore.AutoScaling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [types-aiobotocore-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-autoscaling-2.9.0/types_aiobotocore_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-2.9.1/types_aiobotocore_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

