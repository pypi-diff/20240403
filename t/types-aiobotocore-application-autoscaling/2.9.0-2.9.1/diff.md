# Comparing `tmp/types-aiobotocore-application-autoscaling-2.9.0.tar.gz` & `tmp/types-aiobotocore-application-autoscaling-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-autoscaling-2.9.0.tar", last modified: Wed Dec 13 19:58:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-autoscaling-2.9.1.tar", last modified: Thu Jan 18 01:20:03 2024, max compression
```

## Comparing `types-aiobotocore-application-autoscaling-2.9.0.tar` & `types-aiobotocore-application-autoscaling-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.978092 types-aiobotocore-application-autoscaling-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14464 2023-12-13 19:58:34.978092 types-aiobotocore-application-autoscaling-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:34.978092 types-aiobotocore-application-autoscaling-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.974092 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16913 2023-12-13 19:41:06.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16912 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:05.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.978092 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14464 2023-12-13 19:58:34.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-13 19:58:34.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:34.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:34.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:34.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-13 19:58:34.000000 types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.049514 types-aiobotocore-application-autoscaling-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14484 2024-01-18 01:20:03.045514 types-aiobotocore-application-autoscaling-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:03.049514 types-aiobotocore-application-autoscaling-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.045514 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-01-18 01:03:04.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-01-18 01:03:04.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-01-18 01:03:04.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-01-18 01:03:04.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-01-18 01:03:04.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:03.045514 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14484 2024-01-18 01:20:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-18 01:20:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-18 01:20:03.000000 types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/LICENSE` & `types-aiobotocore-application-autoscaling-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-autoscaling
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
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
 
 <a id="types-aiobotocore-application-autoscaling"></a>
 
 # types-aiobotocore-application-autoscaling
 
 [![PyPI - types-aiobotocore-application-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationAutoScaling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[aiobotocore.ApplicationAutoScaling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/README.md` & `types-aiobotocore-application-autoscaling-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationAutoScaling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[aiobotocore.ApplicationAutoScaling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/setup.py` & `types-aiobotocore-application-autoscaling-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-autoscaling",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationAutoScaling 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ApplicationAutoScaling 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore application-autoscaling type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_application_autoscaling": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/__init__.py` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     DescribeScalingActivitiesPaginator,
     DescribeScalingPoliciesPaginator,
     DescribeScheduledActionsPaginator,
 )
 
 Client = ApplicationAutoScalingClient
 
-
 __all__ = (
     "ApplicationAutoScalingClient",
     "Client",
     "DescribeScalableTargetsPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScalingPoliciesPaginator",
     "DescribeScheduledActionsPaginator",
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/__init__.pyi` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/__main__.py` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationAutoScaling 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationAutoScaling 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/client.py` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationAutoScalingClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -108,15 +107,15 @@
 
     async def delete_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
-        ScalableDimension: ScalableDimensionType
+        ScalableDimension: ScalableDimensionType,
     ) -> Dict[str, Any]:
         """
         Deletes the specified scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#delete_scaling_policy)
@@ -124,30 +123,30 @@
 
     async def delete_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
-        ScalableDimension: ScalableDimensionType
+        ScalableDimension: ScalableDimensionType,
     ) -> Dict[str, Any]:
         """
         Deletes the specified scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#delete_scheduled_action)
         """
 
     async def deregister_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
-        ScalableDimension: ScalableDimensionType
+        ScalableDimension: ScalableDimensionType,
     ) -> Dict[str, Any]:
         """
         Deregisters an Application Auto Scaling scalable target when you have finished
         using
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.deregister_scalable_target)
@@ -157,15 +156,15 @@
     async def describe_scalable_targets(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalableTargetsResponseTypeDef:
         """
         Gets information about the scalable targets in the specified namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scalable_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#describe_scalable_targets)
         """
@@ -174,15 +173,15 @@
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        IncludeNotScaledActivities: bool = ...
+        IncludeNotScaledActivities: bool = ...,
     ) -> DescribeScalingActivitiesResponseTypeDef:
         """
         Provides descriptive information about the scaling activities in the specified
         namespace from the previous six
         weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_activities)
@@ -193,15 +192,15 @@
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalingPoliciesResponseTypeDef:
         """
         Describes the Application Auto Scaling scaling policies for the specified
         service
         namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_policies)
@@ -212,15 +211,15 @@
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScheduledActionsResponseTypeDef:
         """
         Describes the Application Auto Scaling scheduled actions for the specified
         service
         namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scheduled_actions)
@@ -256,15 +255,15 @@
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
         StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...,
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scaling_policy)
@@ -277,15 +276,15 @@
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         Schedule: str = ...,
         Timezone: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        ScalableTargetAction: ScalableTargetActionTypeDef = ...
+        ScalableTargetAction: ScalableTargetActionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scheduled_action)
@@ -297,15 +296,15 @@
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
         MaxCapacity: int = ...,
         RoleARN: str = ...,
         SuspendedState: SuspendedStateTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> RegisterScalableTargetResponseTypeDef:
         """
         Registers or updates a scalable target, which is the resource that you want to
         scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#register_scalable_target)
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/client.pyi` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     async def delete_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
-        ScalableDimension: ScalableDimensionType
+        ScalableDimension: ScalableDimensionType,
     ) -> Dict[str, Any]:
         """
         Deletes the specified scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#delete_scaling_policy)
@@ -120,30 +120,30 @@
 
     async def delete_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
-        ScalableDimension: ScalableDimensionType
+        ScalableDimension: ScalableDimensionType,
     ) -> Dict[str, Any]:
         """
         Deletes the specified scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#delete_scheduled_action)
         """
 
     async def deregister_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
-        ScalableDimension: ScalableDimensionType
+        ScalableDimension: ScalableDimensionType,
     ) -> Dict[str, Any]:
         """
         Deregisters an Application Auto Scaling scalable target when you have finished
         using
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.deregister_scalable_target)
@@ -153,15 +153,15 @@
     async def describe_scalable_targets(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalableTargetsResponseTypeDef:
         """
         Gets information about the scalable targets in the specified namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scalable_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#describe_scalable_targets)
         """
@@ -170,15 +170,15 @@
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        IncludeNotScaledActivities: bool = ...
+        IncludeNotScaledActivities: bool = ...,
     ) -> DescribeScalingActivitiesResponseTypeDef:
         """
         Provides descriptive information about the scaling activities in the specified
         namespace from the previous six
         weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_activities)
@@ -189,15 +189,15 @@
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScalingPoliciesResponseTypeDef:
         """
         Describes the Application Auto Scaling scaling policies for the specified
         service
         namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_policies)
@@ -208,15 +208,15 @@
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeScheduledActionsResponseTypeDef:
         """
         Describes the Application Auto Scaling scheduled actions for the specified
         service
         namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scheduled_actions)
@@ -252,15 +252,15 @@
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
         StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...,
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scaling_policy)
@@ -273,15 +273,15 @@
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         Schedule: str = ...,
         Timezone: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        ScalableTargetAction: ScalableTargetActionTypeDef = ...
+        ScalableTargetAction: ScalableTargetActionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scheduled_action)
@@ -293,15 +293,15 @@
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
         MaxCapacity: int = ...,
         RoleARN: str = ...,
         SuspendedState: SuspendedStateTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> RegisterScalableTargetResponseTypeDef:
         """
         Registers or updates a scalable target, which is the resource that you want to
         scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#register_scalable_target)
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/literals.py` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/literals.py`

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
     "AdjustmentTypeType",
     "DescribeScalableTargetsPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScalingPoliciesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "MetricAggregationTypeType",
@@ -36,15 +35,14 @@
     "ApplicationAutoScalingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
 DescribeScalableTargetsPaginatorName = Literal["describe_scalable_targets"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScalingPoliciesPaginatorName = Literal["describe_scaling_policies"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 MetricAggregationTypeType = Literal["Average", "Maximum", "Minimum"]
 MetricStatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/literals.pyi` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/paginator.py` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "DescribeScalableTargetsPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScalingPoliciesPaginator",
     "DescribeScheduledActionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -67,15 +66,15 @@
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
 
@@ -88,15 +87,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 
@@ -109,15 +108,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
 
@@ -130,13 +129,13 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/paginator.pyi` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
 class DescribeScalingActivitiesPaginator(AioPaginator):
@@ -84,15 +84,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 class DescribeScalingPoliciesPaginator(AioPaginator):
@@ -104,15 +104,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
 class DescribeScheduledActionsPaginator(AioPaginator):
@@ -124,13 +124,13 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/type_defs.py` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/type_defs.py`

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
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling/type_defs.pyi` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-autoscaling
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
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
 
 <a id="types-aiobotocore-application-autoscaling"></a>
 
 # types-aiobotocore-application-autoscaling
 
 [![PyPI - types-aiobotocore-application-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationAutoScaling 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[aiobotocore.ApplicationAutoScaling 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-application-autoscaling-2.9.0/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-application-autoscaling-2.9.1/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

