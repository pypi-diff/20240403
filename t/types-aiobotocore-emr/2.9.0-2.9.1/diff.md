# Comparing `tmp/types-aiobotocore-emr-2.9.0.tar.gz` & `tmp/types-aiobotocore-emr-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-2.9.0.tar", last modified: Wed Dec 13 19:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-2.9.1.tar", last modified: Thu Jan 18 01:20:41 2024, max compression
```

## Comparing `types-aiobotocore-emr-2.9.0.tar` & `types-aiobotocore-emr-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.429753 types-aiobotocore-emr-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14991 2023-12-13 19:59:16.429753 types-aiobotocore-emr-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13444 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:16.429753 types-aiobotocore-emr-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.429753 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46858 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46854 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    74374 2023-12-13 19:45:56.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    74373 2023-12-13 19:45:55.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-12-13 19:45:54.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:16.429753 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14991 2023-12-13 19:59:16.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:16.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:16.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:16.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:16.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:16.000000 types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.133340 types-aiobotocore-emr-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2024-01-18 01:20:41.133340 types-aiobotocore-emr-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:41.133340 types-aiobotocore-emr-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.129341 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46873 2024-01-18 01:07:49.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46870 2024-01-18 01:07:49.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-01-18 01:07:50.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-01-18 01:07:50.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12842 2024-01-18 01:07:50.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-01-18 01:07:50.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    74373 2024-01-18 01:07:51.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74373 2024-01-18 01:07:51.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:48.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-01-18 01:07:50.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-01-18 01:07:50.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:41.133340 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2024-01-18 01:20:41.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:41.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:41.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:41.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:41.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:41.000000 types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-2.9.0/LICENSE` & `types-aiobotocore-emr-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-emr-2.9.0/PKG-INFO` & `types-aiobotocore-emr-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EMR 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EMR 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/
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
 
 <a id="types-aiobotocore-emr"></a>
 
 # types-aiobotocore-emr
 
 [![PyPI - types-aiobotocore-emr](https://img.shields.io/pypi/v/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr)](https://pepy.tech/project/types-aiobotocore-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMR 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[aiobotocore.EMR 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [types-aiobotocore-emr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-2.9.0/README.md` & `types-aiobotocore-emr-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr)](https://pepy.tech/project/types-aiobotocore-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMR 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[aiobotocore.EMR 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [types-aiobotocore-emr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-2.9.0/setup.py` & `types-aiobotocore-emr-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMR 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.EMR 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore emr type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_emr": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/__init__.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 Client = EMRClient
 
-
 __all__ = (
     "Client",
     "ClusterRunningWaiter",
     "ClusterTerminatedWaiter",
     "EMRClient",
     "ListBootstrapActionsPaginator",
     "ListClustersPaginator",
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/__init__.pyi` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/__main__.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMR 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EMR 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/client.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EMRClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -197,15 +196,15 @@
         """
 
     async def cancel_steps(
         self,
         *,
         ClusterId: str,
         StepIds: Sequence[str],
-        StepCancellationOption: StepCancellationOptionType = ...
+        StepCancellationOption: StepCancellationOptionType = ...,
     ) -> CancelStepsOutputTypeDef:
         """
         Cancels a pending step or steps in a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.cancel_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#cancel_steps)
         """
@@ -245,15 +244,15 @@
         UserRole: str = ...,
         IdpAuthUrl: str = ...,
         IdpRelayStateParameterName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TrustedIdentityPropagationEnabled: bool = ...,
         IdcUserAssignment: IdcUserAssignmentType = ...,
         IdcInstanceArn: str = ...,
-        EncryptionKeyArn: str = ...
+        EncryptionKeyArn: str = ...,
     ) -> CreateStudioOutputTypeDef:
         """
         Creates a new Amazon EMR Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#create_studio)
         """
@@ -261,15 +260,15 @@
     async def create_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         SessionPolicyArn: str,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Maps a user or group to the Amazon EMR Studio specified by `StudioId`, and
         applies a session policy to refine Studio permissions for that user or
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio_session_mapping)
@@ -294,15 +293,15 @@
 
     async def delete_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a user or group from an Amazon EMR Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.delete_studio_session_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#delete_studio_session_mapping)
         """
@@ -319,15 +318,15 @@
 
     async def describe_job_flows(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         JobFlowIds: Sequence[str] = ...,
-        JobFlowStates: Sequence[JobFlowExecutionStateType] = ...
+        JobFlowStates: Sequence[JobFlowExecutionStateType] = ...,
     ) -> DescribeJobFlowsOutputTypeDef:
         """
         This API is no longer supported and will eventually be removed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_job_flows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#describe_job_flows)
         """
@@ -444,15 +443,15 @@
 
     async def get_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> GetStudioSessionMappingOutputTypeDef:
         """
         Fetches mapping details for the specified Amazon EMR Studio and identity (user
         or
         group).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_studio_session_mapping)
@@ -471,15 +470,15 @@
 
     async def list_clusters(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ListClustersOutputTypeDef:
         """
         Provides the status of all clusters visible to this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#list_clusters)
         """
@@ -509,15 +508,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ListInstancesOutputTypeDef:
         """
         Provides information for all active Amazon EC2 instances and Amazon EC2
         instances terminated in the last 30 days, up to a maximum of
         2,000.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instances)
@@ -528,29 +527,29 @@
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: TimestampTypeDef = ...,
         To: TimestampTypeDef = ...,
         Marker: str = ...,
-        ExecutionEngineId: str = ...
+        ExecutionEngineId: str = ...,
     ) -> ListNotebookExecutionsOutputTypeDef:
         """
         Provides summaries of all notebook executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#list_notebook_executions)
         """
 
     async def list_release_labels(
         self,
         *,
         Filters: ReleaseLabelFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReleaseLabelsOutputTypeDef:
         """
         Retrieves release labels of Amazon EMR services in the Region where the API is
         called.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_release_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#list_release_labels)
@@ -570,15 +569,15 @@
 
     async def list_steps(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ListStepsOutputTypeDef:
         """
         Provides a list of steps for the cluster in reverse order unless you specify
         `stepIds` with the request or filter by
         `StepStates`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_steps)
@@ -641,15 +640,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#modify_instance_fleet)
         """
 
     async def modify_instance_groups(
         self,
         *,
         ClusterId: str = ...,
-        InstanceGroups: Sequence[InstanceGroupModifyConfigTypeDef] = ...
+        InstanceGroups: Sequence[InstanceGroupModifyConfigTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         ModifyInstanceGroups modifies the number of nodes and configuration settings of
         an instance
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.modify_instance_groups)
@@ -766,15 +765,15 @@
         KerberosAttributes: KerberosAttributesTypeDef = ...,
         StepConcurrencyLevel: int = ...,
         ManagedScalingPolicy: ManagedScalingPolicyTypeDef = ...,
         PlacementGroupConfigs: Sequence[PlacementGroupConfigTypeDef] = ...,
         AutoTerminationPolicy: AutoTerminationPolicyTypeDef = ...,
         OSReleaseLabel: str = ...,
         EbsRootVolumeIops: int = ...,
-        EbsRootVolumeThroughput: int = ...
+        EbsRootVolumeThroughput: int = ...,
     ) -> RunJobFlowOutputTypeDef:
         """
         RunJobFlow creates and starts running a new cluster (job flow).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.run_job_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#run_job_flow)
         """
@@ -812,15 +811,15 @@
         NotebookExecutionName: str = ...,
         NotebookParams: str = ...,
         NotebookInstanceSecurityGroupId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         NotebookS3Location: NotebookS3LocationFromInputTypeDef = ...,
         OutputNotebookS3Location: OutputNotebookS3LocationFromInputTypeDef = ...,
         OutputNotebookFormat: Literal["HTML"] = ...,
-        EnvironmentVariables: Mapping[str, str] = ...
+        EnvironmentVariables: Mapping[str, str] = ...,
     ) -> StartNotebookExecutionOutputTypeDef:
         """
         Starts a notebook execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.start_notebook_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#start_notebook_execution)
         """
@@ -849,15 +848,15 @@
         self,
         *,
         StudioId: str,
         Name: str = ...,
         Description: str = ...,
         SubnetIds: Sequence[str] = ...,
         DefaultS3Location: str = ...,
-        EncryptionKeyArn: str = ...
+        EncryptionKeyArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an Amazon EMR Studio configuration, including attributes such as name,
         description, and
         subnets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.update_studio)
@@ -867,15 +866,15 @@
     async def update_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         SessionPolicyArn: str,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the session policy attached to the user or group for the specified
         Amazon EMR
         Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.update_studio_session_mapping)
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/client.pyi` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         """
 
     async def cancel_steps(
         self,
         *,
         ClusterId: str,
         StepIds: Sequence[str],
-        StepCancellationOption: StepCancellationOptionType = ...
+        StepCancellationOption: StepCancellationOptionType = ...,
     ) -> CancelStepsOutputTypeDef:
         """
         Cancels a pending step or steps in a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.cancel_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#cancel_steps)
         """
@@ -241,15 +241,15 @@
         UserRole: str = ...,
         IdpAuthUrl: str = ...,
         IdpRelayStateParameterName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TrustedIdentityPropagationEnabled: bool = ...,
         IdcUserAssignment: IdcUserAssignmentType = ...,
         IdcInstanceArn: str = ...,
-        EncryptionKeyArn: str = ...
+        EncryptionKeyArn: str = ...,
     ) -> CreateStudioOutputTypeDef:
         """
         Creates a new Amazon EMR Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#create_studio)
         """
@@ -257,15 +257,15 @@
     async def create_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         SessionPolicyArn: str,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Maps a user or group to the Amazon EMR Studio specified by `StudioId`, and
         applies a session policy to refine Studio permissions for that user or
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio_session_mapping)
@@ -290,15 +290,15 @@
 
     async def delete_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a user or group from an Amazon EMR Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.delete_studio_session_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#delete_studio_session_mapping)
         """
@@ -315,15 +315,15 @@
 
     async def describe_job_flows(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         JobFlowIds: Sequence[str] = ...,
-        JobFlowStates: Sequence[JobFlowExecutionStateType] = ...
+        JobFlowStates: Sequence[JobFlowExecutionStateType] = ...,
     ) -> DescribeJobFlowsOutputTypeDef:
         """
         This API is no longer supported and will eventually be removed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_job_flows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#describe_job_flows)
         """
@@ -440,15 +440,15 @@
 
     async def get_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> GetStudioSessionMappingOutputTypeDef:
         """
         Fetches mapping details for the specified Amazon EMR Studio and identity (user
         or
         group).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.get_studio_session_mapping)
@@ -467,15 +467,15 @@
 
     async def list_clusters(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ListClustersOutputTypeDef:
         """
         Provides the status of all clusters visible to this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#list_clusters)
         """
@@ -505,15 +505,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ListInstancesOutputTypeDef:
         """
         Provides information for all active Amazon EC2 instances and Amazon EC2
         instances terminated in the last 30 days, up to a maximum of
         2,000.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instances)
@@ -524,29 +524,29 @@
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: TimestampTypeDef = ...,
         To: TimestampTypeDef = ...,
         Marker: str = ...,
-        ExecutionEngineId: str = ...
+        ExecutionEngineId: str = ...,
     ) -> ListNotebookExecutionsOutputTypeDef:
         """
         Provides summaries of all notebook executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#list_notebook_executions)
         """
 
     async def list_release_labels(
         self,
         *,
         Filters: ReleaseLabelFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListReleaseLabelsOutputTypeDef:
         """
         Retrieves release labels of Amazon EMR services in the Region where the API is
         called.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_release_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#list_release_labels)
@@ -566,15 +566,15 @@
 
     async def list_steps(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ListStepsOutputTypeDef:
         """
         Provides a list of steps for the cluster in reverse order unless you specify
         `stepIds` with the request or filter by
         `StepStates`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_steps)
@@ -637,15 +637,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#modify_instance_fleet)
         """
 
     async def modify_instance_groups(
         self,
         *,
         ClusterId: str = ...,
-        InstanceGroups: Sequence[InstanceGroupModifyConfigTypeDef] = ...
+        InstanceGroups: Sequence[InstanceGroupModifyConfigTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         ModifyInstanceGroups modifies the number of nodes and configuration settings of
         an instance
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.modify_instance_groups)
@@ -762,15 +762,15 @@
         KerberosAttributes: KerberosAttributesTypeDef = ...,
         StepConcurrencyLevel: int = ...,
         ManagedScalingPolicy: ManagedScalingPolicyTypeDef = ...,
         PlacementGroupConfigs: Sequence[PlacementGroupConfigTypeDef] = ...,
         AutoTerminationPolicy: AutoTerminationPolicyTypeDef = ...,
         OSReleaseLabel: str = ...,
         EbsRootVolumeIops: int = ...,
-        EbsRootVolumeThroughput: int = ...
+        EbsRootVolumeThroughput: int = ...,
     ) -> RunJobFlowOutputTypeDef:
         """
         RunJobFlow creates and starts running a new cluster (job flow).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.run_job_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#run_job_flow)
         """
@@ -808,15 +808,15 @@
         NotebookExecutionName: str = ...,
         NotebookParams: str = ...,
         NotebookInstanceSecurityGroupId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         NotebookS3Location: NotebookS3LocationFromInputTypeDef = ...,
         OutputNotebookS3Location: OutputNotebookS3LocationFromInputTypeDef = ...,
         OutputNotebookFormat: Literal["HTML"] = ...,
-        EnvironmentVariables: Mapping[str, str] = ...
+        EnvironmentVariables: Mapping[str, str] = ...,
     ) -> StartNotebookExecutionOutputTypeDef:
         """
         Starts a notebook execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.start_notebook_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#start_notebook_execution)
         """
@@ -845,15 +845,15 @@
         self,
         *,
         StudioId: str,
         Name: str = ...,
         Description: str = ...,
         SubnetIds: Sequence[str] = ...,
         DefaultS3Location: str = ...,
-        EncryptionKeyArn: str = ...
+        EncryptionKeyArn: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an Amazon EMR Studio configuration, including attributes such as name,
         description, and
         subnets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.update_studio)
@@ -863,15 +863,15 @@
     async def update_studio_session_mapping(
         self,
         *,
         StudioId: str,
         IdentityType: IdentityTypeType,
         SessionPolicyArn: str,
         IdentityId: str = ...,
-        IdentityName: str = ...
+        IdentityName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the session policy attached to the user or group for the specified
         Amazon EMR
         Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.update_studio_session_mapping)
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/literals.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/literals.py`

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
     "ActionOnFailureType",
     "AdjustmentTypeType",
     "AuthModeType",
     "AutoScalingPolicyStateChangeReasonCodeType",
     "AutoScalingPolicyStateType",
     "CancelStepsRequestStatusType",
@@ -80,15 +79,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionOnFailureType = Literal[
     "CANCEL_AND_WAIT", "CONTINUE", "TERMINATE_CLUSTER", "TERMINATE_JOB_FLOW"
 ]
 AdjustmentTypeType = Literal["CHANGE_IN_CAPACITY", "EXACT_CAPACITY", "PERCENT_CHANGE_IN_CAPACITY"]
 AuthModeType = Literal["IAM", "SSO"]
 AutoScalingPolicyStateChangeReasonCodeType = Literal[
     "CLEANUP_FAILURE", "PROVISION_FAILURE", "USER_REQUEST"
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/literals.pyi` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/paginator.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     "ListNotebookExecutionsPaginator",
     "ListSecurityConfigurationsPaginator",
     "ListStepsPaginator",
     "ListStudioSessionMappingsPaginator",
     "ListStudiosPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -115,15 +114,15 @@
 
     def paginate(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#listclusterspaginator)
         """
 
 
@@ -168,15 +167,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#listinstancespaginator)
         """
 
 
@@ -190,15 +189,15 @@
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: TimestampTypeDef = ...,
         To: TimestampTypeDef = ...,
         ExecutionEngineId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#listnotebookexecutionspaginator)
         """
 
 
@@ -225,15 +224,15 @@
 
     def paginate(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStepsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#liststepspaginator)
         """
 
 
@@ -244,15 +243,15 @@
     """
 
     def paginate(
         self,
         *,
         StudioId: str = ...,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStudioSessionMappingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#liststudiosessionmappingspaginator)
         """
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/paginator.pyi` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     def paginate(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#listclusterspaginator)
         """
 
 class ListInstanceFleetsPaginator(AioPaginator):
@@ -161,15 +161,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#listinstancespaginator)
         """
 
 class ListNotebookExecutionsPaginator(AioPaginator):
@@ -182,15 +182,15 @@
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: TimestampTypeDef = ...,
         To: TimestampTypeDef = ...,
         ExecutionEngineId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#listnotebookexecutionspaginator)
         """
 
 class ListSecurityConfigurationsPaginator(AioPaginator):
@@ -215,15 +215,15 @@
 
     def paginate(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStepsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#liststepspaginator)
         """
 
 class ListStudioSessionMappingsPaginator(AioPaginator):
@@ -233,15 +233,15 @@
     """
 
     def paginate(
         self,
         *,
         StudioId: str = ...,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStudioSessionMappingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/paginators/#liststudiosessionmappingspaginator)
         """
 
 class ListStudiosPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/type_defs.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplicationTypeDef",
     "ScalingConstraintsTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/type_defs.pyi` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/waiter.py` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr/waiter.pyi` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/PKG-INFO` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EMR 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EMR 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/
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
 
 <a id="types-aiobotocore-emr"></a>
 
 # types-aiobotocore-emr
 
 [![PyPI - types-aiobotocore-emr](https://img.shields.io/pypi/v/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr)](https://pepy.tech/project/types-aiobotocore-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMR 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[aiobotocore.EMR 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [types-aiobotocore-emr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-emr-2.9.0/types_aiobotocore_emr.egg-info/SOURCES.txt` & `types-aiobotocore-emr-2.9.1/types_aiobotocore_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

