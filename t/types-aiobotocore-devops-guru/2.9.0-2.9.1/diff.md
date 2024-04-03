# Comparing `tmp/types-aiobotocore-devops-guru-2.9.0.tar.gz` & `tmp/types-aiobotocore-devops-guru-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devops-guru-2.9.0.tar", last modified: Wed Dec 13 19:59:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-devops-guru-2.9.1.tar", last modified: Thu Jan 18 01:20:31 2024, max compression
```

## Comparing `types-aiobotocore-devops-guru-2.9.0.tar` & `types-aiobotocore-devops-guru-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.077838 types-aiobotocore-devops-guru-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15472 2023-12-13 19:59:06.077838 types-aiobotocore-devops-guru-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13894 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:06.077838 types-aiobotocore-devops-guru-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.073838 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33279 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14580 2023-12-13 19:44:05.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14578 2023-12-13 19:44:05.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19334 2023-12-13 19:44:05.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19318 2023-12-13 19:44:05.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54171 2023-12-13 19:44:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    54170 2023-12-13 19:44:05.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:04.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.073838 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15472 2023-12-13 19:59:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 19:59:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:06.000000 types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.513388 types-aiobotocore-devops-guru-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-01-18 01:20:31.513388 types-aiobotocore-devops-guru-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:31.513388 types-aiobotocore-devops-guru-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.513388 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33294 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33291 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14578 2024-01-18 01:06:00.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14578 2024-01-18 01:06:00.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19344 2024-01-18 01:06:00.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19329 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54170 2024-01-18 01:06:01.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54170 2024-01-18 01:06:00.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:59.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.513388 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-01-18 01:20:31.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:20:31.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:31.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:31.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:31.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:20:31.000000 types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/LICENSE` & `types-aiobotocore-devops-guru-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-devops-guru-2.9.0/PKG-INFO` & `types-aiobotocore-devops-guru-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devops-guru
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DevOpsGuru 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DevOpsGuru 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/
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
 
 <a id="types-aiobotocore-devops-guru"></a>
 
 # types-aiobotocore-devops-guru
 
 [![PyPI - types-aiobotocore-devops-guru](https://img.shields.io/pypi/v/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devops-guru)](https://pepy.tech/project/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DevOpsGuru 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[aiobotocore.DevOpsGuru 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [types-aiobotocore-devops-guru docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/README.md` & `types-aiobotocore-devops-guru-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devops-guru)](https://pepy.tech/project/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DevOpsGuru 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[aiobotocore.DevOpsGuru 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [types-aiobotocore-devops-guru docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/setup.py` & `types-aiobotocore-devops-guru-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devops-guru",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DevOpsGuru 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DevOpsGuru 2.9.1 service generated with"
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
     keywords="aiobotocore devops-guru type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_devops_guru": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/__init__.py` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 
 Client = DevOpsGuruClient
 
-
 __all__ = (
     "Client",
     "DescribeOrganizationResourceCollectionHealthPaginator",
     "DescribeResourceCollectionHealthPaginator",
     "DevOpsGuruClient",
     "GetCostEstimationPaginator",
     "GetResourceCollectionPaginator",
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/__init__.pyi` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/__main__.py` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DevOpsGuru 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DevOpsGuru 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/client.py` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DevOpsGuruClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -242,15 +241,15 @@
 
     async def describe_organization_overview(
         self,
         *,
         FromTime: TimestampTypeDef,
         ToTime: TimestampTypeDef = ...,
         AccountIds: Sequence[str] = ...,
-        OrganizationalUnitIds: Sequence[str] = ...
+        OrganizationalUnitIds: Sequence[str] = ...,
     ) -> DescribeOrganizationOverviewResponseTypeDef:
         """
         Returns an overview of your organization's history based on the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_overview)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_organization_overview)
@@ -259,15 +258,15 @@
     async def describe_organization_resource_collection_health(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeOrganizationResourceCollectionHealthResponseTypeDef:
         """
         Provides an overview of your system's health.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_resource_collection_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_organization_resource_collection_health)
         """
@@ -335,15 +334,15 @@
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         AccountId: str = ...,
-        Filters: ListAnomaliesForInsightFiltersTypeDef = ...
+        Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
     ) -> ListAnomaliesForInsightResponseTypeDef:
         """
         Returns a list of the anomalies that belong to an insight that you specify
         using its
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_anomalies_for_insight)
@@ -362,15 +361,15 @@
 
     async def list_events(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListEventsResponseTypeDef:
         """
         Returns a list of the events emitted by the resources that are evaluated by
         DevOps
         Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_events)
@@ -378,29 +377,29 @@
         """
 
     async def list_insights(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListInsightsResponseTypeDef:
         """
         Returns a list of insights in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#list_insights)
         """
 
     async def list_monitored_resources(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListMonitoredResourcesResponseTypeDef:
         """
         Returns the list of all log groups that are being monitored and tagged by
         DevOps
         Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_monitored_resources)
@@ -420,30 +419,30 @@
     async def list_organization_insights(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         MaxResults: int = ...,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOrganizationInsightsResponseTypeDef:
         """
         Returns a list of insights associated with the account or OU Id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#list_organization_insights)
         """
 
     async def list_recommendations(
         self,
         *,
         InsightId: str,
         NextToken: str = ...,
         Locale: LocaleType = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         Returns a list of a specified insight's recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#list_recommendations)
         """
@@ -469,15 +468,15 @@
     async def search_insights(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchInsightsResponseTypeDef:
         """
         Returns a list of insights in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_insights)
         """
@@ -486,28 +485,28 @@
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchOrganizationInsightsResponseTypeDef:
         """
         Returns a list of insights in your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_organization_insights)
         """
 
     async def start_cost_estimation(
         self,
         *,
         ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
@@ -526,15 +525,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#update_event_sources_config)
         """
 
     async def update_resource_collection(
         self,
         *,
         Action: UpdateResourceCollectionActionType,
-        ResourceCollection: UpdateResourceCollectionFilterTypeDef
+        ResourceCollection: UpdateResourceCollectionFilterTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates the collection of resources that DevOps Guru analyzes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.update_resource_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#update_resource_collection)
         """
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/client.pyi` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
     async def describe_organization_overview(
         self,
         *,
         FromTime: TimestampTypeDef,
         ToTime: TimestampTypeDef = ...,
         AccountIds: Sequence[str] = ...,
-        OrganizationalUnitIds: Sequence[str] = ...
+        OrganizationalUnitIds: Sequence[str] = ...,
     ) -> DescribeOrganizationOverviewResponseTypeDef:
         """
         Returns an overview of your organization's history based on the specified time
         range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_overview)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_organization_overview)
@@ -255,15 +255,15 @@
     async def describe_organization_resource_collection_health(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeOrganizationResourceCollectionHealthResponseTypeDef:
         """
         Provides an overview of your system's health.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_resource_collection_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_organization_resource_collection_health)
         """
@@ -331,15 +331,15 @@
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         AccountId: str = ...,
-        Filters: ListAnomaliesForInsightFiltersTypeDef = ...
+        Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
     ) -> ListAnomaliesForInsightResponseTypeDef:
         """
         Returns a list of the anomalies that belong to an insight that you specify
         using its
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_anomalies_for_insight)
@@ -358,15 +358,15 @@
 
     async def list_events(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         MaxResults: int = ...,
         NextToken: str = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListEventsResponseTypeDef:
         """
         Returns a list of the events emitted by the resources that are evaluated by
         DevOps
         Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_events)
@@ -374,29 +374,29 @@
         """
 
     async def list_insights(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListInsightsResponseTypeDef:
         """
         Returns a list of insights in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#list_insights)
         """
 
     async def list_monitored_resources(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListMonitoredResourcesResponseTypeDef:
         """
         Returns the list of all log groups that are being monitored and tagged by
         DevOps
         Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_monitored_resources)
@@ -416,30 +416,30 @@
     async def list_organization_insights(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         MaxResults: int = ...,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOrganizationInsightsResponseTypeDef:
         """
         Returns a list of insights associated with the account or OU Id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#list_organization_insights)
         """
 
     async def list_recommendations(
         self,
         *,
         InsightId: str,
         NextToken: str = ...,
         Locale: LocaleType = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         Returns a list of a specified insight's recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#list_recommendations)
         """
@@ -465,15 +465,15 @@
     async def search_insights(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchInsightsResponseTypeDef:
         """
         Returns a list of insights in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_insights)
         """
@@ -482,28 +482,28 @@
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchOrganizationInsightsResponseTypeDef:
         """
         Returns a list of insights in your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_organization_insights)
         """
 
     async def start_cost_estimation(
         self,
         *,
         ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
@@ -522,15 +522,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#update_event_sources_config)
         """
 
     async def update_resource_collection(
         self,
         *,
         Action: UpdateResourceCollectionActionType,
-        ResourceCollection: UpdateResourceCollectionFilterTypeDef
+        ResourceCollection: UpdateResourceCollectionFilterTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates the collection of resources that DevOps Guru analyzes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.update_resource_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#update_resource_collection)
         """
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/literals.py` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/literals.py`

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
     "AnomalySeverityType",
     "AnomalyStatusType",
     "AnomalyTypeType",
     "CloudWatchMetricDataStatusCodeType",
     "CloudWatchMetricsStatType",
     "CostEstimationServiceResourceStateType",
@@ -63,15 +62,14 @@
     "DevOpsGuruServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnomalySeverityType = Literal["HIGH", "LOW", "MEDIUM"]
 AnomalyStatusType = Literal["CLOSED", "ONGOING"]
 AnomalyTypeType = Literal["CAUSAL", "CONTEXTUAL"]
 CloudWatchMetricDataStatusCodeType = Literal["Complete", "InternalError", "PartialData"]
 CloudWatchMetricsStatType = Literal[
     "Average", "Maximum", "Minimum", "SampleCount", "Sum", "p50", "p90", "p99"
 ]
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/literals.pyi` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/paginator.py` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     "ListNotificationChannelsPaginator",
     "ListOrganizationInsightsPaginator",
     "ListRecommendationsPaginator",
     "SearchInsightsPaginator",
     "SearchOrganizationInsightsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -120,15 +119,15 @@
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
 
@@ -138,15 +137,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
 
@@ -171,15 +170,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
 
@@ -192,15 +191,15 @@
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
 
@@ -226,15 +225,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listeventspaginator)
         """
 
 
@@ -244,15 +243,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
         """
 
 
@@ -262,15 +261,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
 
@@ -297,15 +296,15 @@
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
 
@@ -317,15 +316,15 @@
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listrecommendationspaginator)
         """
 
 
@@ -337,15 +336,15 @@
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchinsightspaginator)
         """
 
 
@@ -358,13 +357,13 @@
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/paginator.pyi` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
 class DescribeResourceCollectionHealthPaginator(AioPaginator):
@@ -134,15 +134,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
 class GetCostEstimationPaginator(AioPaginator):
@@ -165,15 +165,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
 class ListAnomaliesForInsightPaginator(AioPaginator):
@@ -185,15 +185,15 @@
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
 class ListAnomalousLogGroupsPaginator(AioPaginator):
@@ -217,15 +217,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listeventspaginator)
         """
 
 class ListInsightsPaginator(AioPaginator):
@@ -234,15 +234,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
         """
 
 class ListMonitoredResourcesPaginator(AioPaginator):
@@ -251,15 +251,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
 class ListNotificationChannelsPaginator(AioPaginator):
@@ -284,15 +284,15 @@
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
 class ListRecommendationsPaginator(AioPaginator):
@@ -303,15 +303,15 @@
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listrecommendationspaginator)
         """
 
 class SearchInsightsPaginator(AioPaginator):
@@ -322,15 +322,15 @@
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchinsightspaginator)
         """
 
 class SearchOrganizationInsightsPaginator(AioPaginator):
@@ -342,13 +342,13 @@
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/type_defs.py` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInsightHealthTypeDef",
     "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru/type_defs.pyi` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/PKG-INFO` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devops-guru
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DevOpsGuru 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DevOpsGuru 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/
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
 
 <a id="types-aiobotocore-devops-guru"></a>
 
 # types-aiobotocore-devops-guru
 
 [![PyPI - types-aiobotocore-devops-guru](https://img.shields.io/pypi/v/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devops-guru)](https://pepy.tech/project/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DevOpsGuru 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[aiobotocore.DevOpsGuru 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [types-aiobotocore-devops-guru docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-devops-guru-2.9.0/types_aiobotocore_devops_guru.egg-info/SOURCES.txt` & `types-aiobotocore-devops-guru-2.9.1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

