# Comparing `tmp/types-aiobotocore-rolesanywhere-2.9.0.tar.gz` & `tmp/types-aiobotocore-rolesanywhere-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rolesanywhere-2.9.0.tar", last modified: Wed Dec 13 20:00:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-rolesanywhere-2.9.1.tar", last modified: Thu Jan 18 01:21:39 2024, max compression
```

## Comparing `types-aiobotocore-rolesanywhere-2.9.0.tar` & `types-aiobotocore-rolesanywhere-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.621231 types-aiobotocore-rolesanywhere-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2023-12-13 20:00:19.621231 types-aiobotocore-rolesanywhere-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12094 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:19.621231 types-aiobotocore-rolesanywhere-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.621231 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22255 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22251 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2023-12-13 19:54:48.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2023-12-13 19:54:48.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2023-12-13 19:54:48.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:47.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.621231 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2023-12-13 20:00:19.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 20:00:19.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:19.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:19.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:19.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 20:00:19.000000 types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.025079 types-aiobotocore-rolesanywhere-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-01-18 01:21:39.025079 types-aiobotocore-rolesanywhere-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:39.025079 types-aiobotocore-rolesanywhere-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.021078 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22259 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22256 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-01-18 01:16:21.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-01-18 01:16:21.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-01-18 01:16:21.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-01-18 01:16:21.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:20.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.025079 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-01-18 01:21:38.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:38.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:38.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:38.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:38.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:38.000000 types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/LICENSE` & `types-aiobotocore-rolesanywhere-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
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
 
 <a id="types-aiobotocore-rolesanywhere"></a>
 
 # types-aiobotocore-rolesanywhere
 
 [![PyPI - types-aiobotocore-rolesanywhere](https://img.shields.io/pypi/v/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAMRolesAnywhere 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[aiobotocore.IAMRolesAnywhere 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/README.md` & `types-aiobotocore-rolesanywhere-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAMRolesAnywhere 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[aiobotocore.IAMRolesAnywhere 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/setup.py` & `types-aiobotocore-rolesanywhere-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rolesanywhere",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IAMRolesAnywhere 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.IAMRolesAnywhere 2.9.1 service generated with"
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
     keywords="aiobotocore rolesanywhere type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rolesanywhere": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/__init__.py` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListProfilesPaginator,
     ListSubjectsPaginator,
     ListTrustAnchorsPaginator,
 )
 
 Client = IAMRolesAnywhereClient
 
-
 __all__ = (
     "Client",
     "IAMRolesAnywhereClient",
     "ListCrlsPaginator",
     "ListProfilesPaginator",
     "ListSubjectsPaginator",
     "ListTrustAnchorsPaginator",
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/__init__.pyi` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/__main__.py` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAMRolesAnywhere 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IAMRolesAnywhere 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/client.py` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IAMRolesAnywhereClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -110,15 +109,15 @@
         name: str,
         roleArns: Sequence[str],
         durationSeconds: int = ...,
         enabled: bool = ...,
         managedPolicyArns: Sequence[str] = ...,
         requireInstanceProperties: bool = ...,
         sessionPolicy: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ProfileDetailResponseTypeDef:
         """
         Creates a *profile*, a list of the roles that Roles Anywhere service is trusted
         to
         assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_profile)
@@ -128,15 +127,15 @@
     async def create_trust_anchor(
         self,
         *,
         name: str,
         source: SourceTypeDef,
         enabled: bool = ...,
         notificationSettings: Sequence[NotificationSettingTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> TrustAnchorDetailResponseTypeDef:
         """
         Creates a trust anchor to establish trust between IAM Roles Anywhere and your
         certificate authority
         (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_trust_anchor)
@@ -265,15 +264,15 @@
     async def import_crl(
         self,
         *,
         crlData: BlobTypeDef,
         name: str,
         trustAnchorArn: str,
         enabled: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CrlDetailResponseTypeDef:
         """
         Imports the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.import_crl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#import_crl)
         """
@@ -341,15 +340,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#put_notification_settings)
         """
 
     async def reset_notification_settings(
         self,
         *,
         notificationSettingKeys: Sequence[NotificationSettingKeyTypeDef],
-        trustAnchorId: str
+        trustAnchorId: str,
     ) -> ResetNotificationSettingsResponseTypeDef:
         """
         Resets the *custom notification setting* to IAM Roles Anywhere default setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.reset_notification_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#reset_notification_settings)
         """
@@ -384,15 +383,15 @@
         self,
         *,
         profileId: str,
         durationSeconds: int = ...,
         managedPolicyArns: Sequence[str] = ...,
         name: str = ...,
         roleArns: Sequence[str] = ...,
-        sessionPolicy: str = ...
+        sessionPolicy: str = ...,
     ) -> ProfileDetailResponseTypeDef:
         """
         Updates a *profile*, a list of the roles that IAM Roles Anywhere service is
         trusted to
         assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_profile)
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/client.pyi` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         name: str,
         roleArns: Sequence[str],
         durationSeconds: int = ...,
         enabled: bool = ...,
         managedPolicyArns: Sequence[str] = ...,
         requireInstanceProperties: bool = ...,
         sessionPolicy: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ProfileDetailResponseTypeDef:
         """
         Creates a *profile*, a list of the roles that Roles Anywhere service is trusted
         to
         assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_profile)
@@ -124,15 +124,15 @@
     async def create_trust_anchor(
         self,
         *,
         name: str,
         source: SourceTypeDef,
         enabled: bool = ...,
         notificationSettings: Sequence[NotificationSettingTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> TrustAnchorDetailResponseTypeDef:
         """
         Creates a trust anchor to establish trust between IAM Roles Anywhere and your
         certificate authority
         (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.create_trust_anchor)
@@ -261,15 +261,15 @@
     async def import_crl(
         self,
         *,
         crlData: BlobTypeDef,
         name: str,
         trustAnchorArn: str,
         enabled: bool = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CrlDetailResponseTypeDef:
         """
         Imports the certificate revocation list (CRL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.import_crl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#import_crl)
         """
@@ -337,15 +337,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#put_notification_settings)
         """
 
     async def reset_notification_settings(
         self,
         *,
         notificationSettingKeys: Sequence[NotificationSettingKeyTypeDef],
-        trustAnchorId: str
+        trustAnchorId: str,
     ) -> ResetNotificationSettingsResponseTypeDef:
         """
         Resets the *custom notification setting* to IAM Roles Anywhere default setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.reset_notification_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/client/#reset_notification_settings)
         """
@@ -380,15 +380,15 @@
         self,
         *,
         profileId: str,
         durationSeconds: int = ...,
         managedPolicyArns: Sequence[str] = ...,
         name: str = ...,
         roleArns: Sequence[str] = ...,
-        sessionPolicy: str = ...
+        sessionPolicy: str = ...,
     ) -> ProfileDetailResponseTypeDef:
         """
         Updates a *profile*, a list of the roles that IAM Roles Anywhere service is
         trusted to
         assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client.update_profile)
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/literals.py` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/literals.py`

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
     "ListCrlsPaginatorName",
     "ListProfilesPaginatorName",
     "ListSubjectsPaginatorName",
     "ListTrustAnchorsPaginatorName",
     "NotificationChannelType",
     "NotificationEventType",
@@ -31,15 +30,14 @@
     "IAMRolesAnywhereServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListCrlsPaginatorName = Literal["list_crls"]
 ListProfilesPaginatorName = Literal["list_profiles"]
 ListSubjectsPaginatorName = Literal["list_subjects"]
 ListTrustAnchorsPaginatorName = Literal["list_trust_anchors"]
 NotificationChannelType = Literal["ALL"]
 NotificationEventType = Literal["CA_CERTIFICATE_EXPIRY", "END_ENTITY_CERTIFICATE_EXPIRY"]
 TrustAnchorTypeType = Literal["AWS_ACM_PCA", "CERTIFICATE_BUNDLE", "SELF_SIGNED_REPOSITORY"]
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/literals.pyi` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/paginator.py` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListCrlsPaginator",
     "ListProfilesPaginator",
     "ListSubjectsPaginator",
     "ListTrustAnchorsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/paginator.pyi` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/type_defs.py` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere/type_defs.pyi` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
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
 
 <a id="types-aiobotocore-rolesanywhere"></a>
 
 # types-aiobotocore-rolesanywhere
 
 [![PyPI - types-aiobotocore-rolesanywhere](https://img.shields.io/pypi/v/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAMRolesAnywhere 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[aiobotocore.IAMRolesAnywhere 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rolesanywhere-2.9.0/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt` & `types-aiobotocore-rolesanywhere-2.9.1/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

