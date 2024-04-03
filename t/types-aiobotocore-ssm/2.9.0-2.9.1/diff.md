# Comparing `tmp/types-aiobotocore-ssm-2.9.0.tar.gz` & `tmp/types-aiobotocore-ssm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-2.9.0.tar", last modified: Wed Dec 13 20:00:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-2.9.1.tar", last modified: Thu Jan 18 01:21:53 2024, max compression
```

## Comparing `types-aiobotocore-ssm-2.9.0.tar` & `types-aiobotocore-ssm-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.889091 types-aiobotocore-ssm-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22030 2023-12-13 20:00:35.889091 types-aiobotocore-ssm-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20483 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:35.889091 types-aiobotocore-ssm-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:56:45.000000 types-aiobotocore-ssm-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.889091 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137298 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   137294 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28774 2023-12-13 19:56:47.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    28772 2023-12-13 19:56:47.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    61625 2023-12-13 19:56:47.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    61576 2023-12-13 19:56:47.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   191837 2023-12-13 19:56:53.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   191836 2023-12-13 19:56:52.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:46.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-13 19:56:47.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-12-13 19:56:47.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.889091 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22030 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.741012 types-aiobotocore-ssm-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-01-18 01:21:53.741012 types-aiobotocore-ssm-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20483 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:53.741012 types-aiobotocore-ssm-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.737012 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137367 2024-01-18 01:18:19.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137364 2024-01-18 01:18:15.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28772 2024-01-18 01:18:20.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28772 2024-01-18 01:18:20.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    61662 2024-01-18 01:18:20.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61614 2024-01-18 01:18:20.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   191836 2024-01-18 01:18:23.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   191836 2024-01-18 01:18:22.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:14.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-01-18 01:18:20.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-01-18 01:18:20.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.737012 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-2.9.0/LICENSE` & `types-aiobotocore-ssm-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ssm-2.9.0/PKG-INFO` & `types-aiobotocore-ssm-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
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
 
 <a id="types-aiobotocore-ssm"></a>
 
 # types-aiobotocore-ssm
 
 [![PyPI - types-aiobotocore-ssm](https://img.shields.io/pypi/v/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[aiobotocore.SSM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [types-aiobotocore-ssm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-2.9.0/README.md` & `types-aiobotocore-ssm-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[aiobotocore.SSM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [types-aiobotocore-ssm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-2.9.0/setup.py` & `types-aiobotocore-ssm-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSM 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SSM 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ssm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ssm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/__init__.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .waiter import CommandExecutedWaiter
 
 Client = SSMClient
 
-
 __all__ = (
     "Client",
     "CommandExecutedWaiter",
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/__init__.pyi` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/__main__.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSM 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SSM 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/client.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,14 @@
 from .waiter import CommandExecutedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -441,15 +440,15 @@
         """
 
     async def add_tags_to_resource(
         self,
         *,
         ResourceType: ResourceTypeForTaggingType,
         ResourceId: str,
-        Tags: Sequence[TagTypeDef]
+        Tags: Sequence[TagTypeDef],
     ) -> Dict[str, Any]:
         """
         Adds or overwrites one or more tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.add_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#add_tags_to_resource)
         """
@@ -507,15 +506,15 @@
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
         ExpirationDate: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...
+        RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...,
     ) -> CreateActivationResultTypeDef:
         """
         Generates an activation code and activation ID you can use to register your
         on-premises servers, edge devices, or virtual machine (VM) with Amazon Web
         Services Systems
         Manager.
 
@@ -541,15 +540,15 @@
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
         TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed
         nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
@@ -576,15 +575,15 @@
         Requires: Sequence[DocumentRequiresTypeDef] = ...,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
         VersionName: str = ...,
         DocumentType: DocumentTypeType = ...,
         DocumentFormat: DocumentFormatType = ...,
         TargetType: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDocumentResultTypeDef:
         """
         Creates a Amazon Web Services Systems Manager (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_document)
         """
@@ -599,15 +598,15 @@
         AllowUnassociatedTargets: bool,
         Description: str = ...,
         StartDate: str = ...,
         EndDate: str = ...,
         ScheduleTimezone: str = ...,
         ScheduleOffset: int = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMaintenanceWindowResultTypeDef:
         """
         Creates a new maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_maintenance_window)
         """
@@ -626,29 +625,29 @@
         Tags: Sequence[TagTypeDef] = ...,
         Category: str = ...,
         Severity: str = ...,
         ActualStartTime: TimestampTypeDef = ...,
         ActualEndTime: TimestampTypeDef = ...,
         PlannedStartTime: TimestampTypeDef = ...,
         PlannedEndTime: TimestampTypeDef = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_item)
         """
 
     async def create_ops_metadata(
         self,
         *,
         ResourceId: str,
         Metadata: Mapping[str, MetadataValueTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOpsMetadataResultTypeDef:
         """
         If you create a new application in Application Manager, Amazon Web Services
         Systems Manager calls this API operation to specify information about the new
         application, including the application
         type.
 
@@ -667,30 +666,30 @@
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
         Sources: Sequence[PatchSourceTypeDef] = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_patch_baseline)
         """
 
     async def create_resource_data_sync(
         self,
         *,
         SyncName: str,
         S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,
         SyncType: str = ...,
-        SyncSource: ResourceDataSyncSourceTypeDef = ...
+        SyncSource: ResourceDataSyncSourceTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         A resource data sync helps you view data from multiple sources in a single
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_resource_data_sync)
@@ -730,15 +729,15 @@
 
     async def delete_inventory(
         self,
         *,
         TypeName: str,
         SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,
         DryRun: bool = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> DeleteInventoryResultTypeDef:
         """
         Delete a custom inventory type or the data associated with a custom Inventory
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_inventory)
@@ -853,15 +852,15 @@
         """
 
     async def describe_activations(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeActivationsResultTypeDef:
         """
         Describes details about the activation, such as the date and time the
         activation was created, its expiration date, the Identity and Access Management
         (IAM) role assigned to the managed nodes in the activation, and the number of
         nodes registered by using this
         activation.
@@ -872,15 +871,15 @@
 
     async def describe_association(
         self,
         *,
         Name: str = ...,
         InstanceId: str = ...,
         AssociationId: str = ...,
-        AssociationVersion: str = ...
+        AssociationVersion: str = ...,
     ) -> DescribeAssociationResultTypeDef:
         """
         Describes the association for the specified target or managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association)
         """
@@ -888,44 +887,44 @@
     async def describe_association_execution_targets(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAssociationExecutionTargetsResultTypeDef:
         """
         Views information about a specific execution of a specific association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_execution_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_execution_targets)
         """
 
     async def describe_association_executions(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAssociationExecutionsResultTypeDef:
         """
         Views all executions for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_executions)
         """
 
     async def describe_automation_executions(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAutomationExecutionsResultTypeDef:
         """
         Provides details about all active and terminated Automation executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_executions)
         """
@@ -933,30 +932,30 @@
     async def describe_automation_step_executions(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ReverseOrder: bool = ...
+        ReverseOrder: bool = ...,
     ) -> DescribeAutomationStepExecutionsResultTypeDef:
         """
         Information about all active and terminated step executions in an Automation
         workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_step_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_step_executions)
         """
 
     async def describe_available_patches(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAvailablePatchesResultTypeDef:
         """
         Lists all patches eligible to be included in a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_available_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_available_patches)
         """
@@ -974,15 +973,15 @@
 
     async def describe_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDocumentPermissionResponseTypeDef:
         """
         Describes the permissions for a Amazon Web Services Systems Manager document
         (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document_permission)
@@ -1023,15 +1022,15 @@
 
     async def describe_instance_information(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeInstanceInformationResultTypeDef:
         """
         Provides information about one or more of your managed nodes, including the
         operating system platform, SSM Agent version, association status, and IP
         address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
@@ -1050,15 +1049,15 @@
 
     async def describe_instance_patch_states_for_patch_group(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeInstancePatchStatesForPatchGroupResultTypeDef:
         """
         Retrieves the high-level patch state for the managed nodes in the specified
         patch
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states_for_patch_group)
@@ -1067,15 +1066,15 @@
 
     async def describe_instance_patches(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeInstancePatchesResultTypeDef:
         """
         Retrieves information about the patches on the specified managed node and their
         state relative to the patch baseline being used for the
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
@@ -1095,15 +1094,15 @@
     async def describe_maintenance_window_execution_task_invocations(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef:
         """
         Retrieves the individual task executions (one per target) for a particular task
         run as part of a maintenance window
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_task_invocations)
@@ -1112,30 +1111,30 @@
 
     async def describe_maintenance_window_execution_tasks(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
         """
         For a given maintenance window execution, lists the tasks that were run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_tasks)
         """
 
     async def describe_maintenance_window_executions(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowExecutionsResultTypeDef:
         """
         Lists the executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_executions)
         """
@@ -1144,74 +1143,74 @@
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_schedule)
         """
 
     async def describe_maintenance_window_targets(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowTargetsResultTypeDef:
         """
         Lists the targets registered with the maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_targets)
         """
 
     async def describe_maintenance_window_tasks(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowTasksResultTypeDef:
         """
         Lists the tasks in a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_tasks)
         """
 
     async def describe_maintenance_windows(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowsResultTypeDef:
         """
         Retrieves the maintenance windows in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows)
         """
 
     async def describe_maintenance_windows_for_target(
         self,
         *,
         Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated
         with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows_for_target)
@@ -1219,44 +1218,44 @@
         """
 
     async def describe_ops_items(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOpsItemsResponseTypeDef:
         """
         Query a set of OpsItems.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_ops_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_ops_items)
         """
 
     async def describe_parameters(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeParametersResultTypeDef:
         """
         Get information about a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_parameters)
         """
 
     async def describe_patch_baselines(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePatchBaselinesResultTypeDef:
         """
         Lists the patch baselines in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_baselines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_baselines)
         """
@@ -1273,15 +1272,15 @@
         """
 
     async def describe_patch_groups(
         self,
         *,
         MaxResults: int = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePatchGroupsResultTypeDef:
         """
         Lists all patch groups that have been registered with patch baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_groups)
         """
@@ -1289,15 +1288,15 @@
     async def describe_patch_properties(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePatchPropertiesResultTypeDef:
         """
         Lists the properties of available patches organized by product, product family,
         classification, severity, and other properties of available
         patches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_properties)
@@ -1306,15 +1305,15 @@
 
     async def describe_sessions(
         self,
         *,
         State: SessionStateType,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[SessionFilterTypeDef] = ...
+        Filters: Sequence[SessionFilterTypeDef] = ...,
     ) -> DescribeSessionsResponseTypeDef:
         """
         Retrieves a list of all active sessions (both connected and disconnected) or
         terminated sessions from the past 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_sessions)
@@ -1410,15 +1409,15 @@
 
     async def get_document(
         self,
         *,
         Name: str,
         VersionName: str = ...,
         DocumentVersion: str = ...,
-        DocumentFormat: DocumentFormatType = ...
+        DocumentFormat: DocumentFormatType = ...,
     ) -> GetDocumentResultTypeDef:
         """
         Gets the contents of the specified Amazon Web Services Systems Manager document
         (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_document)
@@ -1428,15 +1427,15 @@
     async def get_inventory(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetInventoryResultTypeDef:
         """
         Query inventory information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory)
         """
@@ -1444,15 +1443,15 @@
     async def get_inventory_schema(
         self,
         *,
         TypeName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Aggregator: bool = ...,
-        SubType: bool = ...
+        SubType: bool = ...,
     ) -> GetInventorySchemaResultTypeDef:
         """
         Return a list of inventory type names for the account, or return a list of
         attribute names for a specific Inventory item
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory_schema)
@@ -1532,15 +1531,15 @@
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetOpsSummaryResultTypeDef:
         """
         View a summary of operations metadata (OpsData) based on specified filters and
         aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_summary)
@@ -1581,15 +1580,15 @@
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetParametersByPathResultTypeDef:
         """
         Retrieve information about one or more parameters in a specific hierarchy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters_by_path)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters_by_path)
         """
@@ -1653,15 +1652,15 @@
         """
 
     async def list_associations(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAssociationsResultTypeDef:
         """
         Returns all State Manager associations in the current Amazon Web Services
         account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_associations)
@@ -1672,15 +1671,15 @@
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        Details: bool = ...
+        Details: bool = ...,
     ) -> ListCommandInvocationsResultTypeDef:
         """
         An invocation is copy of a command sent to a specific managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_command_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_command_invocations)
         """
@@ -1688,15 +1687,15 @@
     async def list_commands(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[CommandFilterTypeDef] = ...
+        Filters: Sequence[CommandFilterTypeDef] = ...,
     ) -> ListCommandsResultTypeDef:
         """
         Lists the commands requested by users of the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_commands)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_commands)
         """
@@ -1704,15 +1703,15 @@
     async def list_compliance_items(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListComplianceItemsResultTypeDef:
         """
         For a specified resource ID, this API operation returns a list of compliance
         statuses for different resource
         types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_items)
@@ -1720,15 +1719,15 @@
         """
 
     async def list_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListComplianceSummariesResultTypeDef:
         """
         Returns a summary count of compliant and non-compliant resources for a
         compliance
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_summaries)
@@ -1738,15 +1737,15 @@
     async def list_document_metadata_history(
         self,
         *,
         Name: str,
         Metadata: Literal["DocumentReviews"],
         DocumentVersion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDocumentMetadataHistoryResponseTypeDef:
         """
         Information about approval reviews for a version of a change template in Change
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_metadata_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_metadata_history)
@@ -1764,15 +1763,15 @@
 
     async def list_documents(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDocumentsResultTypeDef:
         """
         Returns all Systems Manager (SSM) documents in the current Amazon Web Services
         account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_documents)
@@ -1782,29 +1781,29 @@
     async def list_inventory_entries(
         self,
         *,
         InstanceId: str,
         TypeName: str,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInventoryEntriesResultTypeDef:
         """
         A list of inventory items returned by the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_inventory_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_inventory_entries)
         """
 
     async def list_ops_item_events(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOpsItemEventsResponseTypeDef:
         """
         Returns a list of all OpsItem events in the current Amazon Web Services Region
         and Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_events)
@@ -1813,30 +1812,30 @@
 
     async def list_ops_item_related_items(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOpsItemRelatedItemsResponseTypeDef:
         """
         Lists all related-item resources associated with a Systems Manager OpsCenter
         OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_related_items)
         """
 
     async def list_ops_metadata(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when displaying
         all Application Manager OpsMetadata objects or
         blobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_metadata)
@@ -1844,15 +1843,15 @@
         """
 
     async def list_resource_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListResourceComplianceSummariesResultTypeDef:
         """
         Returns a resource-level summary count.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_compliance_summaries)
         """
@@ -1880,15 +1879,15 @@
     async def modify_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         AccountIdsToAdd: Sequence[str] = ...,
         AccountIdsToRemove: Sequence[str] = ...,
-        SharedDocumentVersion: str = ...
+        SharedDocumentVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
         privately.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.modify_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#modify_document_permission)
@@ -1899,15 +1898,15 @@
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
         ExecutionSummary: ComplianceExecutionSummaryTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
-        UploadType: ComplianceUploadTypeType = ...
+        UploadType: ComplianceUploadTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_compliance_items)
@@ -1932,15 +1931,15 @@
         Type: ParameterTypeType = ...,
         KeyId: str = ...,
         Overwrite: bool = ...,
         AllowedPattern: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Tier: ParameterTierType = ...,
         Policies: str = ...,
-        DataType: str = ...
+        DataType: str = ...,
     ) -> PutParameterResultTypeDef:
         """
         Add a parameter to the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_parameter)
         """
@@ -1980,15 +1979,15 @@
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
         Targets: Sequence[TargetTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_target_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_target_with_maintenance_window)
         """
@@ -2007,15 +2006,15 @@
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_task_with_maintenance_window)
         """
@@ -2047,15 +2046,15 @@
         """
 
     async def send_automation_signal(
         self,
         *,
         AutomationExecutionId: str,
         SignalType: SignalTypeType,
-        Payload: Mapping[str, Sequence[str]] = ...
+        Payload: Mapping[str, Sequence[str]] = ...,
     ) -> Dict[str, Any]:
         """
         Sends a signal to an Automation execution to change the current behavior or
         status of the
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_automation_signal)
@@ -2078,15 +2077,15 @@
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
         NotificationConfig: NotificationConfigTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_command)
         """
@@ -2110,15 +2109,15 @@
         TargetParameterName: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_automation_execution)
         """
@@ -2132,30 +2131,30 @@
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ScheduledEndTime: TimestampTypeDef = ...,
-        ChangeDetails: str = ...
+        ChangeDetails: str = ...,
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_change_request_execution)
         """
 
     async def start_session(
         self,
         *,
         Target: str,
         DocumentName: str = ...,
         Reason: str = ...,
-        Parameters: Mapping[str, Sequence[str]] = ...
+        Parameters: Mapping[str, Sequence[str]] = ...,
     ) -> StartSessionResponseTypeDef:
         """
         Initiates a connection to a target (for example, a managed node) for a Session
         Manager
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_session)
@@ -2210,15 +2209,15 @@
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
         TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association)
         """
@@ -2241,15 +2240,15 @@
         Content: str,
         Name: str,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
         VersionName: str = ...,
         DocumentVersion: str = ...,
         DocumentFormat: DocumentFormatType = ...,
-        TargetType: str = ...
+        TargetType: str = ...,
     ) -> UpdateDocumentResultTypeDef:
         """
         Updates one or more values for an SSM document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document)
         """
@@ -2287,15 +2286,15 @@
         Schedule: str = ...,
         ScheduleTimezone: str = ...,
         ScheduleOffset: int = ...,
         Duration: int = ...,
         Cutoff: int = ...,
         AllowUnassociatedTargets: bool = ...,
         Enabled: bool = ...,
-        Replace: bool = ...
+        Replace: bool = ...,
     ) -> UpdateMaintenanceWindowResultTypeDef:
         """
         Updates an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window)
         """
@@ -2305,15 +2304,15 @@
         *,
         WindowId: str,
         WindowTargetId: str,
         Targets: Sequence[TargetTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
-        Replace: bool = ...
+        Replace: bool = ...,
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_target)
         """
@@ -2332,15 +2331,15 @@
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_task)
         """
@@ -2371,29 +2370,29 @@
         Title: str = ...,
         Category: str = ...,
         Severity: str = ...,
         ActualStartTime: TimestampTypeDef = ...,
         ActualEndTime: TimestampTypeDef = ...,
         PlannedStartTime: TimestampTypeDef = ...,
         PlannedEndTime: TimestampTypeDef = ...,
-        OpsItemArn: str = ...
+        OpsItemArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_item)
         """
 
     async def update_ops_metadata(
         self,
         *,
         OpsMetadataArn: str,
         MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,
-        KeysToDelete: Sequence[str] = ...
+        KeysToDelete: Sequence[str] = ...,
     ) -> UpdateOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when you edit
         OpsMetadata in Application
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_metadata)
@@ -2410,15 +2409,15 @@
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
         Sources: Sequence[PatchSourceTypeDef] = ...,
-        Replace: bool = ...
+        Replace: bool = ...,
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_patch_baseline)
         """
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/client.pyi` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,15 @@
         """
 
     async def add_tags_to_resource(
         self,
         *,
         ResourceType: ResourceTypeForTaggingType,
         ResourceId: str,
-        Tags: Sequence[TagTypeDef]
+        Tags: Sequence[TagTypeDef],
     ) -> Dict[str, Any]:
         """
         Adds or overwrites one or more tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.add_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#add_tags_to_resource)
         """
@@ -503,15 +503,15 @@
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
         ExpirationDate: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...
+        RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...,
     ) -> CreateActivationResultTypeDef:
         """
         Generates an activation code and activation ID you can use to register your
         on-premises servers, edge devices, or virtual machine (VM) with Amazon Web
         Services Systems
         Manager.
 
@@ -537,15 +537,15 @@
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
         TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed
         nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
@@ -572,15 +572,15 @@
         Requires: Sequence[DocumentRequiresTypeDef] = ...,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
         VersionName: str = ...,
         DocumentType: DocumentTypeType = ...,
         DocumentFormat: DocumentFormatType = ...,
         TargetType: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDocumentResultTypeDef:
         """
         Creates a Amazon Web Services Systems Manager (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_document)
         """
@@ -595,15 +595,15 @@
         AllowUnassociatedTargets: bool,
         Description: str = ...,
         StartDate: str = ...,
         EndDate: str = ...,
         ScheduleTimezone: str = ...,
         ScheduleOffset: int = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMaintenanceWindowResultTypeDef:
         """
         Creates a new maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_maintenance_window)
         """
@@ -622,29 +622,29 @@
         Tags: Sequence[TagTypeDef] = ...,
         Category: str = ...,
         Severity: str = ...,
         ActualStartTime: TimestampTypeDef = ...,
         ActualEndTime: TimestampTypeDef = ...,
         PlannedStartTime: TimestampTypeDef = ...,
         PlannedEndTime: TimestampTypeDef = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_item)
         """
 
     async def create_ops_metadata(
         self,
         *,
         ResourceId: str,
         Metadata: Mapping[str, MetadataValueTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOpsMetadataResultTypeDef:
         """
         If you create a new application in Application Manager, Amazon Web Services
         Systems Manager calls this API operation to specify information about the new
         application, including the application
         type.
 
@@ -663,30 +663,30 @@
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
         Sources: Sequence[PatchSourceTypeDef] = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_patch_baseline)
         """
 
     async def create_resource_data_sync(
         self,
         *,
         SyncName: str,
         S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,
         SyncType: str = ...,
-        SyncSource: ResourceDataSyncSourceTypeDef = ...
+        SyncSource: ResourceDataSyncSourceTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         A resource data sync helps you view data from multiple sources in a single
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_resource_data_sync)
@@ -726,15 +726,15 @@
 
     async def delete_inventory(
         self,
         *,
         TypeName: str,
         SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,
         DryRun: bool = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> DeleteInventoryResultTypeDef:
         """
         Delete a custom inventory type or the data associated with a custom Inventory
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_inventory)
@@ -849,15 +849,15 @@
         """
 
     async def describe_activations(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeActivationsResultTypeDef:
         """
         Describes details about the activation, such as the date and time the
         activation was created, its expiration date, the Identity and Access Management
         (IAM) role assigned to the managed nodes in the activation, and the number of
         nodes registered by using this
         activation.
@@ -868,15 +868,15 @@
 
     async def describe_association(
         self,
         *,
         Name: str = ...,
         InstanceId: str = ...,
         AssociationId: str = ...,
-        AssociationVersion: str = ...
+        AssociationVersion: str = ...,
     ) -> DescribeAssociationResultTypeDef:
         """
         Describes the association for the specified target or managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association)
         """
@@ -884,44 +884,44 @@
     async def describe_association_execution_targets(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAssociationExecutionTargetsResultTypeDef:
         """
         Views information about a specific execution of a specific association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_execution_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_execution_targets)
         """
 
     async def describe_association_executions(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAssociationExecutionsResultTypeDef:
         """
         Views all executions for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_executions)
         """
 
     async def describe_automation_executions(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAutomationExecutionsResultTypeDef:
         """
         Provides details about all active and terminated Automation executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_executions)
         """
@@ -929,30 +929,30 @@
     async def describe_automation_step_executions(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ReverseOrder: bool = ...
+        ReverseOrder: bool = ...,
     ) -> DescribeAutomationStepExecutionsResultTypeDef:
         """
         Information about all active and terminated step executions in an Automation
         workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_step_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_step_executions)
         """
 
     async def describe_available_patches(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeAvailablePatchesResultTypeDef:
         """
         Lists all patches eligible to be included in a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_available_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_available_patches)
         """
@@ -970,15 +970,15 @@
 
     async def describe_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDocumentPermissionResponseTypeDef:
         """
         Describes the permissions for a Amazon Web Services Systems Manager document
         (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document_permission)
@@ -1019,15 +1019,15 @@
 
     async def describe_instance_information(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeInstanceInformationResultTypeDef:
         """
         Provides information about one or more of your managed nodes, including the
         operating system platform, SSM Agent version, association status, and IP
         address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
@@ -1046,15 +1046,15 @@
 
     async def describe_instance_patch_states_for_patch_group(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeInstancePatchStatesForPatchGroupResultTypeDef:
         """
         Retrieves the high-level patch state for the managed nodes in the specified
         patch
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states_for_patch_group)
@@ -1063,15 +1063,15 @@
 
     async def describe_instance_patches(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeInstancePatchesResultTypeDef:
         """
         Retrieves information about the patches on the specified managed node and their
         state relative to the patch baseline being used for the
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
@@ -1091,15 +1091,15 @@
     async def describe_maintenance_window_execution_task_invocations(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef:
         """
         Retrieves the individual task executions (one per target) for a particular task
         run as part of a maintenance window
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_task_invocations)
@@ -1108,30 +1108,30 @@
 
     async def describe_maintenance_window_execution_tasks(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
         """
         For a given maintenance window execution, lists the tasks that were run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_tasks)
         """
 
     async def describe_maintenance_window_executions(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowExecutionsResultTypeDef:
         """
         Lists the executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_executions)
         """
@@ -1140,74 +1140,74 @@
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_schedule)
         """
 
     async def describe_maintenance_window_targets(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowTargetsResultTypeDef:
         """
         Lists the targets registered with the maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_targets)
         """
 
     async def describe_maintenance_window_tasks(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowTasksResultTypeDef:
         """
         Lists the tasks in a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_tasks)
         """
 
     async def describe_maintenance_windows(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowsResultTypeDef:
         """
         Retrieves the maintenance windows in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows)
         """
 
     async def describe_maintenance_windows_for_target(
         self,
         *,
         Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated
         with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows_for_target)
@@ -1215,44 +1215,44 @@
         """
 
     async def describe_ops_items(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeOpsItemsResponseTypeDef:
         """
         Query a set of OpsItems.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_ops_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_ops_items)
         """
 
     async def describe_parameters(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeParametersResultTypeDef:
         """
         Get information about a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_parameters)
         """
 
     async def describe_patch_baselines(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePatchBaselinesResultTypeDef:
         """
         Lists the patch baselines in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_baselines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_baselines)
         """
@@ -1269,15 +1269,15 @@
         """
 
     async def describe_patch_groups(
         self,
         *,
         MaxResults: int = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePatchGroupsResultTypeDef:
         """
         Lists all patch groups that have been registered with patch baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_groups)
         """
@@ -1285,15 +1285,15 @@
     async def describe_patch_properties(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePatchPropertiesResultTypeDef:
         """
         Lists the properties of available patches organized by product, product family,
         classification, severity, and other properties of available
         patches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_properties)
@@ -1302,15 +1302,15 @@
 
     async def describe_sessions(
         self,
         *,
         State: SessionStateType,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[SessionFilterTypeDef] = ...
+        Filters: Sequence[SessionFilterTypeDef] = ...,
     ) -> DescribeSessionsResponseTypeDef:
         """
         Retrieves a list of all active sessions (both connected and disconnected) or
         terminated sessions from the past 30
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_sessions)
@@ -1406,15 +1406,15 @@
 
     async def get_document(
         self,
         *,
         Name: str,
         VersionName: str = ...,
         DocumentVersion: str = ...,
-        DocumentFormat: DocumentFormatType = ...
+        DocumentFormat: DocumentFormatType = ...,
     ) -> GetDocumentResultTypeDef:
         """
         Gets the contents of the specified Amazon Web Services Systems Manager document
         (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_document)
@@ -1424,15 +1424,15 @@
     async def get_inventory(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetInventoryResultTypeDef:
         """
         Query inventory information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory)
         """
@@ -1440,15 +1440,15 @@
     async def get_inventory_schema(
         self,
         *,
         TypeName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Aggregator: bool = ...,
-        SubType: bool = ...
+        SubType: bool = ...,
     ) -> GetInventorySchemaResultTypeDef:
         """
         Return a list of inventory type names for the account, or return a list of
         attribute names for a specific Inventory item
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory_schema)
@@ -1528,15 +1528,15 @@
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetOpsSummaryResultTypeDef:
         """
         View a summary of operations metadata (OpsData) based on specified filters and
         aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_summary)
@@ -1577,15 +1577,15 @@
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetParametersByPathResultTypeDef:
         """
         Retrieve information about one or more parameters in a specific hierarchy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters_by_path)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters_by_path)
         """
@@ -1649,15 +1649,15 @@
         """
 
     async def list_associations(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAssociationsResultTypeDef:
         """
         Returns all State Manager associations in the current Amazon Web Services
         account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_associations)
@@ -1668,15 +1668,15 @@
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        Details: bool = ...
+        Details: bool = ...,
     ) -> ListCommandInvocationsResultTypeDef:
         """
         An invocation is copy of a command sent to a specific managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_command_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_command_invocations)
         """
@@ -1684,15 +1684,15 @@
     async def list_commands(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[CommandFilterTypeDef] = ...
+        Filters: Sequence[CommandFilterTypeDef] = ...,
     ) -> ListCommandsResultTypeDef:
         """
         Lists the commands requested by users of the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_commands)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_commands)
         """
@@ -1700,15 +1700,15 @@
     async def list_compliance_items(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListComplianceItemsResultTypeDef:
         """
         For a specified resource ID, this API operation returns a list of compliance
         statuses for different resource
         types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_items)
@@ -1716,15 +1716,15 @@
         """
 
     async def list_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListComplianceSummariesResultTypeDef:
         """
         Returns a summary count of compliant and non-compliant resources for a
         compliance
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_summaries)
@@ -1734,15 +1734,15 @@
     async def list_document_metadata_history(
         self,
         *,
         Name: str,
         Metadata: Literal["DocumentReviews"],
         DocumentVersion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDocumentMetadataHistoryResponseTypeDef:
         """
         Information about approval reviews for a version of a change template in Change
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_metadata_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_metadata_history)
@@ -1760,15 +1760,15 @@
 
     async def list_documents(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDocumentsResultTypeDef:
         """
         Returns all Systems Manager (SSM) documents in the current Amazon Web Services
         account and Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_documents)
@@ -1778,29 +1778,29 @@
     async def list_inventory_entries(
         self,
         *,
         InstanceId: str,
         TypeName: str,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInventoryEntriesResultTypeDef:
         """
         A list of inventory items returned by the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_inventory_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_inventory_entries)
         """
 
     async def list_ops_item_events(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOpsItemEventsResponseTypeDef:
         """
         Returns a list of all OpsItem events in the current Amazon Web Services Region
         and Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_events)
@@ -1809,30 +1809,30 @@
 
     async def list_ops_item_related_items(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOpsItemRelatedItemsResponseTypeDef:
         """
         Lists all related-item resources associated with a Systems Manager OpsCenter
         OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_related_items)
         """
 
     async def list_ops_metadata(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when displaying
         all Application Manager OpsMetadata objects or
         blobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_metadata)
@@ -1840,15 +1840,15 @@
         """
 
     async def list_resource_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListResourceComplianceSummariesResultTypeDef:
         """
         Returns a resource-level summary count.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_compliance_summaries)
         """
@@ -1876,15 +1876,15 @@
     async def modify_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         AccountIdsToAdd: Sequence[str] = ...,
         AccountIdsToRemove: Sequence[str] = ...,
-        SharedDocumentVersion: str = ...
+        SharedDocumentVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
         privately.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.modify_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#modify_document_permission)
@@ -1895,15 +1895,15 @@
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
         ExecutionSummary: ComplianceExecutionSummaryTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
-        UploadType: ComplianceUploadTypeType = ...
+        UploadType: ComplianceUploadTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_compliance_items)
@@ -1928,15 +1928,15 @@
         Type: ParameterTypeType = ...,
         KeyId: str = ...,
         Overwrite: bool = ...,
         AllowedPattern: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Tier: ParameterTierType = ...,
         Policies: str = ...,
-        DataType: str = ...
+        DataType: str = ...,
     ) -> PutParameterResultTypeDef:
         """
         Add a parameter to the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_parameter)
         """
@@ -1976,15 +1976,15 @@
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
         Targets: Sequence[TargetTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_target_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_target_with_maintenance_window)
         """
@@ -2003,15 +2003,15 @@
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_task_with_maintenance_window)
         """
@@ -2043,15 +2043,15 @@
         """
 
     async def send_automation_signal(
         self,
         *,
         AutomationExecutionId: str,
         SignalType: SignalTypeType,
-        Payload: Mapping[str, Sequence[str]] = ...
+        Payload: Mapping[str, Sequence[str]] = ...,
     ) -> Dict[str, Any]:
         """
         Sends a signal to an Automation execution to change the current behavior or
         status of the
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_automation_signal)
@@ -2074,15 +2074,15 @@
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
         NotificationConfig: NotificationConfigTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_command)
         """
@@ -2106,15 +2106,15 @@
         TargetParameterName: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_automation_execution)
         """
@@ -2128,30 +2128,30 @@
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ScheduledEndTime: TimestampTypeDef = ...,
-        ChangeDetails: str = ...
+        ChangeDetails: str = ...,
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_change_request_execution)
         """
 
     async def start_session(
         self,
         *,
         Target: str,
         DocumentName: str = ...,
         Reason: str = ...,
-        Parameters: Mapping[str, Sequence[str]] = ...
+        Parameters: Mapping[str, Sequence[str]] = ...,
     ) -> StartSessionResponseTypeDef:
         """
         Initiates a connection to a target (for example, a managed node) for a Session
         Manager
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_session)
@@ -2206,15 +2206,15 @@
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
         TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association)
         """
@@ -2237,15 +2237,15 @@
         Content: str,
         Name: str,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
         VersionName: str = ...,
         DocumentVersion: str = ...,
         DocumentFormat: DocumentFormatType = ...,
-        TargetType: str = ...
+        TargetType: str = ...,
     ) -> UpdateDocumentResultTypeDef:
         """
         Updates one or more values for an SSM document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document)
         """
@@ -2283,15 +2283,15 @@
         Schedule: str = ...,
         ScheduleTimezone: str = ...,
         ScheduleOffset: int = ...,
         Duration: int = ...,
         Cutoff: int = ...,
         AllowUnassociatedTargets: bool = ...,
         Enabled: bool = ...,
-        Replace: bool = ...
+        Replace: bool = ...,
     ) -> UpdateMaintenanceWindowResultTypeDef:
         """
         Updates an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window)
         """
@@ -2301,15 +2301,15 @@
         *,
         WindowId: str,
         WindowTargetId: str,
         Targets: Sequence[TargetTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
-        Replace: bool = ...
+        Replace: bool = ...,
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_target)
         """
@@ -2328,15 +2328,15 @@
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...,
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_task)
         """
@@ -2367,29 +2367,29 @@
         Title: str = ...,
         Category: str = ...,
         Severity: str = ...,
         ActualStartTime: TimestampTypeDef = ...,
         ActualEndTime: TimestampTypeDef = ...,
         PlannedStartTime: TimestampTypeDef = ...,
         PlannedEndTime: TimestampTypeDef = ...,
-        OpsItemArn: str = ...
+        OpsItemArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_item)
         """
 
     async def update_ops_metadata(
         self,
         *,
         OpsMetadataArn: str,
         MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,
-        KeysToDelete: Sequence[str] = ...
+        KeysToDelete: Sequence[str] = ...,
     ) -> UpdateOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when you edit
         OpsMetadata in Application
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_metadata)
@@ -2406,15 +2406,15 @@
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
         Sources: Sequence[PatchSourceTypeDef] = ...,
-        Replace: bool = ...
+        Replace: bool = ...,
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_patch_baseline)
         """
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/literals.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/literals.py`

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
     "AssociationComplianceSeverityType",
     "AssociationExecutionFilterKeyType",
     "AssociationExecutionTargetsFilterKeyType",
     "AssociationFilterKeyType",
     "AssociationFilterOperatorTypeType",
     "AssociationStatusNameType",
@@ -158,15 +157,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AssociationComplianceSeverityType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM", "UNSPECIFIED"]
 AssociationExecutionFilterKeyType = Literal["CreatedTime", "ExecutionId", "Status"]
 AssociationExecutionTargetsFilterKeyType = Literal["ResourceId", "ResourceType", "Status"]
 AssociationFilterKeyType = Literal[
     "AssociationId",
     "AssociationName",
     "AssociationStatusName",
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/literals.pyi` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/paginator.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,14 @@
     "ListOpsItemEventsPaginator",
     "ListOpsItemRelatedItemsPaginator",
     "ListOpsMetadataPaginator",
     "ListResourceComplianceSummariesPaginator",
     "ListResourceDataSyncPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -272,15 +271,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
         """
 
 
@@ -292,15 +291,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 
@@ -311,15 +310,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAssociationExecutionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 
@@ -329,15 +328,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAutomationExecutionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 
@@ -349,15 +348,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAutomationStepExecutionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 
@@ -367,15 +366,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 
@@ -431,15 +430,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 
@@ -465,15 +464,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 
@@ -484,15 +483,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 
@@ -519,15 +518,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 
@@ -538,15 +537,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTasksResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 
@@ -557,15 +556,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 
@@ -578,15 +577,15 @@
     def paginate(
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetPaginatorTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 
@@ -597,15 +596,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowTargetsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 
@@ -616,15 +615,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowTasksResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 
@@ -634,15 +633,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 
@@ -653,15 +652,15 @@
     """
 
     def paginate(
         self,
         *,
         Targets: Sequence[TargetPaginatorTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 
@@ -671,15 +670,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
         """
 
 
@@ -690,15 +689,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeparameterspaginator)
         """
 
 
@@ -708,15 +707,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 
@@ -726,15 +725,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
         """
 
 
@@ -746,15 +745,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 
@@ -765,15 +764,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describesessionspaginator)
         """
 
 
@@ -785,15 +784,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence[InventoryAggregatorTypeDef] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventorypaginator)
         """
 
 
@@ -805,15 +804,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventoryschemapaginator)
         """
 
 
@@ -826,15 +825,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence[OpsAggregatorTypeDef] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getopssummarypaginator)
         """
 
 
@@ -845,15 +844,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparameterhistorypaginator)
         """
 
 
@@ -866,15 +865,15 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparametersbypathpaginator)
         """
 
 
@@ -914,15 +913,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssociationsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
         """
 
 
@@ -935,15 +934,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 
@@ -955,15 +954,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCommandsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandspaginator)
         """
 
 
@@ -975,15 +974,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 
@@ -993,15 +992,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 
@@ -1027,15 +1026,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentspaginator)
         """
 
 
@@ -1045,15 +1044,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
         """
 
 
@@ -1064,15 +1063,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 
@@ -1082,15 +1081,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
         """
 
 
@@ -1100,15 +1099,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/paginator.pyi` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
         """
 
 class DescribeAssociationExecutionTargetsPaginator(AioPaginator):
@@ -288,15 +288,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 class DescribeAssociationExecutionsPaginator(AioPaginator):
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAssociationExecutionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 class DescribeAutomationExecutionsPaginator(AioPaginator):
@@ -323,15 +323,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAutomationExecutionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 class DescribeAutomationStepExecutionsPaginator(AioPaginator):
@@ -342,15 +342,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAutomationStepExecutionsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 class DescribeAvailablePatchesPaginator(AioPaginator):
@@ -359,15 +359,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 class DescribeEffectiveInstanceAssociationsPaginator(AioPaginator):
@@ -419,15 +419,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 class DescribeInstancePatchStatesPaginator(AioPaginator):
@@ -451,15 +451,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 class DescribeInstancePatchesPaginator(AioPaginator):
@@ -469,15 +469,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 class DescribeInventoryDeletionsPaginator(AioPaginator):
@@ -502,15 +502,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTasksPaginator(AioPaginator):
@@ -520,15 +520,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTasksResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionsPaginator(AioPaginator):
@@ -538,15 +538,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 class DescribeMaintenanceWindowSchedulePaginator(AioPaginator):
@@ -558,15 +558,15 @@
     def paginate(
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetPaginatorTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 class DescribeMaintenanceWindowTargetsPaginator(AioPaginator):
@@ -576,15 +576,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowTargetsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 class DescribeMaintenanceWindowTasksPaginator(AioPaginator):
@@ -594,15 +594,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowTasksResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 class DescribeMaintenanceWindowsPaginator(AioPaginator):
@@ -611,15 +611,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 class DescribeMaintenanceWindowsForTargetPaginator(AioPaginator):
@@ -629,15 +629,15 @@
     """
 
     def paginate(
         self,
         *,
         Targets: Sequence[TargetPaginatorTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 class DescribeOpsItemsPaginator(AioPaginator):
@@ -646,15 +646,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
         """
 
 class DescribeParametersPaginator(AioPaginator):
@@ -664,15 +664,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeparameterspaginator)
         """
 
 class DescribePatchBaselinesPaginator(AioPaginator):
@@ -681,15 +681,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 class DescribePatchGroupsPaginator(AioPaginator):
@@ -698,15 +698,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
         """
 
 class DescribePatchPropertiesPaginator(AioPaginator):
@@ -717,15 +717,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 class DescribeSessionsPaginator(AioPaginator):
@@ -735,15 +735,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describesessionspaginator)
         """
 
 class GetInventoryPaginator(AioPaginator):
@@ -754,15 +754,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence[InventoryAggregatorTypeDef] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventorypaginator)
         """
 
 class GetInventorySchemaPaginator(AioPaginator):
@@ -773,15 +773,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventoryschemapaginator)
         """
 
 class GetOpsSummaryPaginator(AioPaginator):
@@ -793,15 +793,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence[OpsAggregatorTypeDef] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getopssummarypaginator)
         """
 
 class GetParameterHistoryPaginator(AioPaginator):
@@ -811,15 +811,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparameterhistorypaginator)
         """
 
 class GetParametersByPathPaginator(AioPaginator):
@@ -831,15 +831,15 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparametersbypathpaginator)
         """
 
 class GetResourcePoliciesPaginator(AioPaginator):
@@ -876,15 +876,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssociationsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
         """
 
 class ListCommandInvocationsPaginator(AioPaginator):
@@ -896,15 +896,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 class ListCommandsPaginator(AioPaginator):
@@ -915,15 +915,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCommandsResultPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandspaginator)
         """
 
 class ListComplianceItemsPaginator(AioPaginator):
@@ -934,15 +934,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 class ListComplianceSummariesPaginator(AioPaginator):
@@ -951,15 +951,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 class ListDocumentVersionsPaginator(AioPaginator):
@@ -983,15 +983,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentspaginator)
         """
 
 class ListOpsItemEventsPaginator(AioPaginator):
@@ -1000,15 +1000,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
         """
 
 class ListOpsItemRelatedItemsPaginator(AioPaginator):
@@ -1018,15 +1018,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 class ListOpsMetadataPaginator(AioPaginator):
@@ -1035,15 +1035,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
         """
 
 class ListResourceComplianceSummariesPaginator(AioPaginator):
@@ -1052,15 +1052,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 class ListResourceDataSyncPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/type_defs.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/type_defs.pyi` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/waiter.py` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,13 +36,13 @@
 
     async def wait(
         self,
         *,
         CommandId: str,
         InstanceId: str,
         PluginName: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Waiter.CommandExecuted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/waiters/#commandexecutedwaiter)
         """
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm/waiter.pyi` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,13 +35,13 @@
 
     async def wait(
         self,
         *,
         CommandId: str,
         InstanceId: str,
         PluginName: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Waiter.CommandExecuted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/waiters/#commandexecutedwaiter)
         """
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/PKG-INFO` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
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
 
 <a id="types-aiobotocore-ssm"></a>
 
 # types-aiobotocore-ssm
 
 [![PyPI - types-aiobotocore-ssm](https://img.shields.io/pypi/v/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[aiobotocore.SSM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [types-aiobotocore-ssm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-2.9.0/types_aiobotocore_ssm.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-2.9.1/types_aiobotocore_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

