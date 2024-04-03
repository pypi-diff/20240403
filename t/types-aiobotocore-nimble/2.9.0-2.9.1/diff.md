# Comparing `tmp/types-aiobotocore-nimble-2.9.0.tar.gz` & `tmp/types-aiobotocore-nimble-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-nimble-2.9.0.tar", last modified: Wed Dec 13 20:00:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-nimble-2.9.1.tar", last modified: Thu Jan 18 01:21:23 2024, max compression
```

## Comparing `types-aiobotocore-nimble-2.9.0.tar` & `types-aiobotocore-nimble-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:02.117383 types-aiobotocore-nimble-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16842 2023-12-13 20:00:02.117383 types-aiobotocore-nimble-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:02.117383 types-aiobotocore-nimble-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:02.117383 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47157 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47153 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18647 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12911 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56980 2023-12-13 19:51:01.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56979 2023-12-13 19:51:01.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2023-12-13 19:50:58.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:02.117383 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16842 2023-12-13 20:00:02.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-13 20:00:02.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:02.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:02.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:02.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 20:00:02.000000 types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:23.237149 types-aiobotocore-nimble-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-01-18 01:21:23.237149 types-aiobotocore-nimble-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:23.237149 types-aiobotocore-nimble-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:23.233149 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47174 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47171 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56979 2024-01-18 01:12:43.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56979 2024-01-18 01:12:42.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:38.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-01-18 01:12:39.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:23.237149 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-01-18 01:21:23.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-18 01:21:23.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:23.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:23.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:23.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:23.000000 types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-nimble-2.9.0/LICENSE` & `types-aiobotocore-nimble-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-nimble-2.9.0/PKG-INFO` & `types-aiobotocore-nimble-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NimbleStudio 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NimbleStudio 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
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
 
 <a id="types-aiobotocore-nimble"></a>
 
 # types-aiobotocore-nimble
 
 [![PyPI - types-aiobotocore-nimble](https://img.shields.io/pypi/v/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [types-aiobotocore-nimble docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-nimble-2.9.0/README.md` & `types-aiobotocore-nimble-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [types-aiobotocore-nimble docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-nimble-2.9.0/setup.py` & `types-aiobotocore-nimble-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-nimble",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NimbleStudio 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.NimbleStudio 2.9.1 service generated with"
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
     keywords="aiobotocore nimble type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_nimble": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/__init__.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
     StudioComponentReadyWaiter,
     StudioDeletedWaiter,
     StudioReadyWaiter,
 )
 
 Client = NimbleStudioClient
 
-
 __all__ = (
     "Client",
     "LaunchProfileDeletedWaiter",
     "LaunchProfileReadyWaiter",
     "ListEulaAcceptancesPaginator",
     "ListEulasPaginator",
     "ListLaunchProfileMembersPaginator",
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/__init__.pyi` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/__main__.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NimbleStudio 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.NimbleStudio 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/client.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NimbleStudioClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -186,15 +185,15 @@
         launchProfileProtocolVersions: Sequence[str],
         name: str,
         streamConfiguration: StreamConfigurationCreateTypeDef,
         studioComponentIds: Sequence[str],
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLaunchProfileResponseTypeDef:
         """
         Create a launch profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_launch_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_launch_profile)
         """
@@ -203,15 +202,15 @@
         self,
         *,
         ec2ImageId: str,
         name: str,
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStreamingImageResponseTypeDef:
         """
         Creates a streaming image resource in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_streaming_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_streaming_image)
         """
@@ -221,30 +220,30 @@
         *,
         launchProfileId: str,
         studioId: str,
         clientToken: str = ...,
         ec2InstanceType: StreamingInstanceTypeType = ...,
         ownedBy: str = ...,
         streamingImageId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStreamingSessionResponseTypeDef:
         """
         Creates a streaming session in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_streaming_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_streaming_session)
         """
 
     async def create_streaming_session_stream(
         self,
         *,
         sessionId: str,
         studioId: str,
         clientToken: str = ...,
-        expirationInSeconds: int = ...
+        expirationInSeconds: int = ...,
     ) -> CreateStreamingSessionStreamResponseTypeDef:
         """
         Creates a streaming session stream for a streaming session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_streaming_session_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_streaming_session_stream)
         """
@@ -254,15 +253,15 @@
         *,
         adminRoleArn: str,
         displayName: str,
         studioName: str,
         userRoleArn: str,
         clientToken: str = ...,
         studioEncryptionConfiguration: StudioEncryptionConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStudioResponseTypeDef:
         """
         Create a new studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_studio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_studio)
         """
@@ -278,15 +277,15 @@
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStudioComponentResponseTypeDef:
         """
         Creates a studio component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_studio_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_studio_component)
         """
@@ -408,15 +407,15 @@
     async def get_launch_profile_initialization(
         self,
         *,
         launchProfileId: str,
         launchProfileProtocolVersions: Sequence[str],
         launchPurpose: str,
         platform: str,
-        studioId: str
+        studioId: str,
     ) -> GetLaunchProfileInitializationResponseTypeDef:
         """
         Get a launch profile initialization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.get_launch_profile_initialization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#get_launch_profile_initialization)
         """
@@ -532,15 +531,15 @@
     async def list_launch_profiles(
         self,
         *,
         studioId: str,
         maxResults: int = ...,
         nextToken: str = ...,
         principalId: str = ...,
-        states: Sequence[LaunchProfileStateType] = ...
+        states: Sequence[LaunchProfileStateType] = ...,
     ) -> ListLaunchProfilesResponseTypeDef:
         """
         List all the launch profiles a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.list_launch_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#list_launch_profiles)
         """
@@ -568,15 +567,15 @@
     async def list_streaming_sessions(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         nextToken: str = ...,
         ownedBy: str = ...,
-        sessionIds: str = ...
+        sessionIds: str = ...,
     ) -> ListStreamingSessionsResponseTypeDef:
         """
         Lists the streaming sessions in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.list_streaming_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#list_streaming_sessions)
         """
@@ -584,15 +583,15 @@
     async def list_studio_components(
         self,
         *,
         studioId: str,
         maxResults: int = ...,
         nextToken: str = ...,
         states: Sequence[StudioComponentStateType] = ...,
-        types: Sequence[StudioComponentTypeType] = ...
+        types: Sequence[StudioComponentTypeType] = ...,
     ) -> ListStudioComponentsResponseTypeDef:
         """
         Lists the `StudioComponents` in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.list_studio_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#list_studio_components)
         """
@@ -630,30 +629,30 @@
     async def put_launch_profile_members(
         self,
         *,
         identityStoreId: str,
         launchProfileId: str,
         members: Sequence[NewLaunchProfileMemberTypeDef],
         studioId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add/update users with given persona to launch profile membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.put_launch_profile_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#put_launch_profile_members)
         """
 
     async def put_studio_members(
         self,
         *,
         identityStoreId: str,
         members: Sequence[NewStudioMemberTypeDef],
         studioId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add/update users with given persona to studio membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.put_studio_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#put_studio_members)
         """
@@ -680,15 +679,15 @@
 
     async def stop_streaming_session(
         self,
         *,
         sessionId: str,
         studioId: str,
         clientToken: str = ...,
-        volumeRetentionMode: VolumeRetentionModeType = ...
+        volumeRetentionMode: VolumeRetentionModeType = ...,
     ) -> StopStreamingSessionResponseTypeDef:
         """
         Transitions sessions from the `READY` state into the `STOPPED` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.stop_streaming_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#stop_streaming_session)
         """
@@ -717,15 +716,15 @@
         launchProfileId: str,
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
         launchProfileProtocolVersions: Sequence[str] = ...,
         name: str = ...,
         streamConfiguration: StreamConfigurationCreateTypeDef = ...,
-        studioComponentIds: Sequence[str] = ...
+        studioComponentIds: Sequence[str] = ...,
     ) -> UpdateLaunchProfileResponseTypeDef:
         """
         Update a launch profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_launch_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_launch_profile)
         """
@@ -733,15 +732,15 @@
     async def update_launch_profile_member(
         self,
         *,
         launchProfileId: str,
         persona: Literal["USER"],
         principalId: str,
         studioId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateLaunchProfileMemberResponseTypeDef:
         """
         Update a user persona in launch profile membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_launch_profile_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_launch_profile_member)
         """
@@ -749,15 +748,15 @@
     async def update_streaming_image(
         self,
         *,
         streamingImageId: str,
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateStreamingImageResponseTypeDef:
         """
         Update streaming image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_streaming_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_streaming_image)
         """
@@ -765,15 +764,15 @@
     async def update_studio(
         self,
         *,
         studioId: str,
         adminRoleArn: str = ...,
         clientToken: str = ...,
         displayName: str = ...,
-        userRoleArn: str = ...
+        userRoleArn: str = ...,
     ) -> UpdateStudioResponseTypeDef:
         """
         Update a Studio resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_studio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_studio)
         """
@@ -789,15 +788,15 @@
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
-        type: StudioComponentTypeType = ...
+        type: StudioComponentTypeType = ...,
     ) -> UpdateStudioComponentResponseTypeDef:
         """
         Updates a studio component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_studio_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_studio_component)
         """
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/client.pyi` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         launchProfileProtocolVersions: Sequence[str],
         name: str,
         streamConfiguration: StreamConfigurationCreateTypeDef,
         studioComponentIds: Sequence[str],
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLaunchProfileResponseTypeDef:
         """
         Create a launch profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_launch_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_launch_profile)
         """
@@ -199,15 +199,15 @@
         self,
         *,
         ec2ImageId: str,
         name: str,
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStreamingImageResponseTypeDef:
         """
         Creates a streaming image resource in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_streaming_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_streaming_image)
         """
@@ -217,30 +217,30 @@
         *,
         launchProfileId: str,
         studioId: str,
         clientToken: str = ...,
         ec2InstanceType: StreamingInstanceTypeType = ...,
         ownedBy: str = ...,
         streamingImageId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStreamingSessionResponseTypeDef:
         """
         Creates a streaming session in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_streaming_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_streaming_session)
         """
 
     async def create_streaming_session_stream(
         self,
         *,
         sessionId: str,
         studioId: str,
         clientToken: str = ...,
-        expirationInSeconds: int = ...
+        expirationInSeconds: int = ...,
     ) -> CreateStreamingSessionStreamResponseTypeDef:
         """
         Creates a streaming session stream for a streaming session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_streaming_session_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_streaming_session_stream)
         """
@@ -250,15 +250,15 @@
         *,
         adminRoleArn: str,
         displayName: str,
         studioName: str,
         userRoleArn: str,
         clientToken: str = ...,
         studioEncryptionConfiguration: StudioEncryptionConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStudioResponseTypeDef:
         """
         Create a new studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_studio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_studio)
         """
@@ -274,15 +274,15 @@
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateStudioComponentResponseTypeDef:
         """
         Creates a studio component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.create_studio_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#create_studio_component)
         """
@@ -404,15 +404,15 @@
     async def get_launch_profile_initialization(
         self,
         *,
         launchProfileId: str,
         launchProfileProtocolVersions: Sequence[str],
         launchPurpose: str,
         platform: str,
-        studioId: str
+        studioId: str,
     ) -> GetLaunchProfileInitializationResponseTypeDef:
         """
         Get a launch profile initialization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.get_launch_profile_initialization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#get_launch_profile_initialization)
         """
@@ -528,15 +528,15 @@
     async def list_launch_profiles(
         self,
         *,
         studioId: str,
         maxResults: int = ...,
         nextToken: str = ...,
         principalId: str = ...,
-        states: Sequence[LaunchProfileStateType] = ...
+        states: Sequence[LaunchProfileStateType] = ...,
     ) -> ListLaunchProfilesResponseTypeDef:
         """
         List all the launch profiles a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.list_launch_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#list_launch_profiles)
         """
@@ -564,15 +564,15 @@
     async def list_streaming_sessions(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         nextToken: str = ...,
         ownedBy: str = ...,
-        sessionIds: str = ...
+        sessionIds: str = ...,
     ) -> ListStreamingSessionsResponseTypeDef:
         """
         Lists the streaming sessions in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.list_streaming_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#list_streaming_sessions)
         """
@@ -580,15 +580,15 @@
     async def list_studio_components(
         self,
         *,
         studioId: str,
         maxResults: int = ...,
         nextToken: str = ...,
         states: Sequence[StudioComponentStateType] = ...,
-        types: Sequence[StudioComponentTypeType] = ...
+        types: Sequence[StudioComponentTypeType] = ...,
     ) -> ListStudioComponentsResponseTypeDef:
         """
         Lists the `StudioComponents` in a studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.list_studio_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#list_studio_components)
         """
@@ -626,30 +626,30 @@
     async def put_launch_profile_members(
         self,
         *,
         identityStoreId: str,
         launchProfileId: str,
         members: Sequence[NewLaunchProfileMemberTypeDef],
         studioId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add/update users with given persona to launch profile membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.put_launch_profile_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#put_launch_profile_members)
         """
 
     async def put_studio_members(
         self,
         *,
         identityStoreId: str,
         members: Sequence[NewStudioMemberTypeDef],
         studioId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Add/update users with given persona to studio membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.put_studio_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#put_studio_members)
         """
@@ -676,15 +676,15 @@
 
     async def stop_streaming_session(
         self,
         *,
         sessionId: str,
         studioId: str,
         clientToken: str = ...,
-        volumeRetentionMode: VolumeRetentionModeType = ...
+        volumeRetentionMode: VolumeRetentionModeType = ...,
     ) -> StopStreamingSessionResponseTypeDef:
         """
         Transitions sessions from the `READY` state into the `STOPPED` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.stop_streaming_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#stop_streaming_session)
         """
@@ -713,15 +713,15 @@
         launchProfileId: str,
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
         launchProfileProtocolVersions: Sequence[str] = ...,
         name: str = ...,
         streamConfiguration: StreamConfigurationCreateTypeDef = ...,
-        studioComponentIds: Sequence[str] = ...
+        studioComponentIds: Sequence[str] = ...,
     ) -> UpdateLaunchProfileResponseTypeDef:
         """
         Update a launch profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_launch_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_launch_profile)
         """
@@ -729,15 +729,15 @@
     async def update_launch_profile_member(
         self,
         *,
         launchProfileId: str,
         persona: Literal["USER"],
         principalId: str,
         studioId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateLaunchProfileMemberResponseTypeDef:
         """
         Update a user persona in launch profile membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_launch_profile_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_launch_profile_member)
         """
@@ -745,15 +745,15 @@
     async def update_streaming_image(
         self,
         *,
         streamingImageId: str,
         studioId: str,
         clientToken: str = ...,
         description: str = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateStreamingImageResponseTypeDef:
         """
         Update streaming image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_streaming_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_streaming_image)
         """
@@ -761,15 +761,15 @@
     async def update_studio(
         self,
         *,
         studioId: str,
         adminRoleArn: str = ...,
         clientToken: str = ...,
         displayName: str = ...,
-        userRoleArn: str = ...
+        userRoleArn: str = ...,
     ) -> UpdateStudioResponseTypeDef:
         """
         Update a Studio resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_studio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_studio)
         """
@@ -785,15 +785,15 @@
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
-        type: StudioComponentTypeType = ...
+        type: StudioComponentTypeType = ...,
     ) -> UpdateStudioComponentResponseTypeDef:
         """
         Updates a studio component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Client.update_studio_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/client/#update_studio_component)
         """
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/literals.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/literals.py`

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
     "AutomaticTerminationModeType",
     "LaunchProfileDeletedWaiterName",
     "LaunchProfilePersonaType",
     "LaunchProfilePlatformType",
     "LaunchProfileReadyWaiterName",
     "LaunchProfileStateType",
@@ -77,15 +76,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AutomaticTerminationModeType = Literal["ACTIVATED", "DEACTIVATED"]
 LaunchProfileDeletedWaiterName = Literal["launch_profile_deleted"]
 LaunchProfilePersonaType = Literal["USER"]
 LaunchProfilePlatformType = Literal["LINUX", "WINDOWS"]
 LaunchProfileReadyWaiterName = Literal["launch_profile_ready"]
 LaunchProfileStateType = Literal[
     "CREATE_FAILED",
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/literals.pyi` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/paginator.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     "ListStreamingSessionBackupsPaginator",
     "ListStreamingSessionsPaginator",
     "ListStudioComponentsPaginator",
     "ListStudioMembersPaginator",
     "ListStudiosPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -90,15 +89,15 @@
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         eulaIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEulaAcceptancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaacceptancespaginator)
         """
 
 
@@ -140,15 +139,15 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         principalId: str = ...,
         states: Sequence[LaunchProfileStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchProfilesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilespaginator)
         """
 
 
@@ -191,15 +190,15 @@
     def paginate(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         ownedBy: str = ...,
         sessionIds: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamingSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionspaginator)
         """
 
 
@@ -211,15 +210,15 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         states: Sequence[StudioComponentStateType] = ...,
         types: Sequence[StudioComponentTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStudioComponentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiocomponentspaginator)
         """
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/paginator.pyi` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """
 
     def paginate(
         self,
         *,
         studioId: str,
         eulaIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEulaAcceptancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListEulaAcceptances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listeulaacceptancespaginator)
         """
 
 class ListEulasPaginator(AioPaginator):
@@ -134,15 +134,15 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         principalId: str = ...,
         states: Sequence[LaunchProfileStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchProfilesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListLaunchProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#listlaunchprofilespaginator)
         """
 
 class ListStreamingImagesPaginator(AioPaginator):
@@ -182,15 +182,15 @@
     def paginate(
         self,
         *,
         studioId: str,
         createdBy: str = ...,
         ownedBy: str = ...,
         sessionIds: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamingSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStreamingSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststreamingsessionspaginator)
         """
 
 class ListStudioComponentsPaginator(AioPaginator):
@@ -201,15 +201,15 @@
 
     def paginate(
         self,
         *,
         studioId: str,
         states: Sequence[StudioComponentStateType] = ...,
         types: Sequence[StudioComponentTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStudioComponentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Paginator.ListStudioComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/paginators/#liststudiocomponentspaginator)
         """
 
 class ListStudioMembersPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/type_defs.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
     "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/type_defs.pyi` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/waiter.py` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     async def wait(
         self,
         *,
         sessionId: str,
         streamId: str,
         studioId: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingSessionStreamReady.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/waiters/#streamingsessionstreamreadywaiter)
         """
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble/waiter.pyi` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
     async def wait(
         self,
         *,
         sessionId: str,
         streamId: str,
         studioId: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio.Waiter.StreamingSessionStreamReady.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/waiters/#streamingsessionstreamreadywaiter)
         """
 
 class StudioComponentDeletedWaiter(AIOWaiter):
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/PKG-INFO` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NimbleStudio 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NimbleStudio 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
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
 
 <a id="types-aiobotocore-nimble"></a>
 
 # types-aiobotocore-nimble
 
 [![PyPI - types-aiobotocore-nimble](https://img.shields.io/pypi/v/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
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
 [types-aiobotocore-nimble docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-nimble-2.9.0/types_aiobotocore_nimble.egg-info/SOURCES.txt` & `types-aiobotocore-nimble-2.9.1/types_aiobotocore_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

