# Comparing `tmp/types-aiobotocore-securitylake-2.9.0.tar.gz` & `tmp/types-aiobotocore-securitylake-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-securitylake-2.9.0.tar", last modified: Wed Dec 13 20:00:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-securitylake-2.9.1.tar", last modified: Thu Jan 18 01:21:47 2024, max compression
```

## Comparing `types-aiobotocore-securitylake-2.9.0.tar` & `types-aiobotocore-securitylake-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:28.757152 types-aiobotocore-securitylake-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2023-12-13 20:00:28.757152 types-aiobotocore-securitylake-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:28.757152 types-aiobotocore-securitylake-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:28.757152 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28083 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28079 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22532 2023-12-13 19:56:15.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22531 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:14.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:28.757152 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2023-12-13 20:00:28.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 20:00:28.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:28.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:28.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:28.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 20:00:28.000000 types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:47.341041 types-aiobotocore-securitylake-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-01-18 01:21:47.341041 types-aiobotocore-securitylake-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:47.341041 types-aiobotocore-securitylake-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:47.341041 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28089 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28086 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22531 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22531 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:44.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:47.341041 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-01-18 01:21:47.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:21:47.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:47.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:47.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:47.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:47.000000 types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-securitylake-2.9.0/LICENSE` & `types-aiobotocore-securitylake-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-securitylake-2.9.0/PKG-INFO` & `types-aiobotocore-securitylake-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SecurityLake 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SecurityLake 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
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
 
 <a id="types-aiobotocore-securitylake"></a>
 
 # types-aiobotocore-securitylake
 
 [![PyPI - types-aiobotocore-securitylake](https://img.shields.io/pypi/v/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityLake 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[aiobotocore.SecurityLake 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-securitylake-2.9.0/README.md` & `types-aiobotocore-securitylake-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityLake 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[aiobotocore.SecurityLake 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-securitylake-2.9.0/setup.py` & `types-aiobotocore-securitylake-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-securitylake",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SecurityLake 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SecurityLake 2.9.1 service generated with"
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
     keywords="aiobotocore securitylake type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_securitylake": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/__init__.py` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDataLakeExceptionsPaginator,
     ListLogSourcesPaginator,
     ListSubscribersPaginator,
 )
 
 Client = SecurityLakeClient
 
-
 __all__ = (
     "Client",
     "GetDataLakeSourcesPaginator",
     "ListDataLakeExceptionsPaginator",
     "ListLogSourcesPaginator",
     "ListSubscribersPaginator",
     "SecurityLakeClient",
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/__init__.pyi` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/__main__.py` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecurityLake 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SecurityLake 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
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

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/client.py` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SecurityLakeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -129,15 +128,15 @@
 
     async def create_custom_log_source(
         self,
         *,
         sourceName: str,
         configuration: CustomLogSourceConfigurationTypeDef = ...,
         eventClasses: Sequence[str] = ...,
-        sourceVersion: str = ...
+        sourceVersion: str = ...,
     ) -> CreateCustomLogSourceResponseTypeDef:
         """
         Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
         Services Region where you want to create a custom
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
@@ -145,30 +144,30 @@
         """
 
     async def create_data_lake(
         self,
         *,
         configurations: Sequence[DataLakeConfigurationTypeDef],
         metaStoreManagerRoleArn: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake)
         """
 
     async def create_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
-        exceptionTimeToLive: int = ...
+        exceptionTimeToLive: int = ...,
     ) -> Dict[str, Any]:
         """
         Creates the specified notification subscription in Amazon Security Lake for the
         organization you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
@@ -190,15 +189,15 @@
         self,
         *,
         sources: Sequence[LogSourceResourceTypeDef],
         subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
         subscriberDescription: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security
         Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
@@ -389,15 +388,15 @@
     async def list_log_sources(
         self,
         *,
         accounts: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regions: Sequence[str] = ...,
-        sources: Sequence[LogSourceResourceTypeDef] = ...
+        sources: Sequence[LogSourceResourceTypeDef] = ...,
     ) -> ListLogSourcesResponseTypeDef:
         """
         Retrieves the log sources in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_log_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_log_sources)
         """
@@ -467,15 +466,15 @@
         """
 
     async def update_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
-        exceptionTimeToLive: int = ...
+        exceptionTimeToLive: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified notification subscription in Amazon Security Lake for the
         organization you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake_exception_subscription)
@@ -485,15 +484,15 @@
     async def update_subscriber(
         self,
         *,
         subscriberId: str,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
         subscriberDescription: str = ...,
         subscriberIdentity: AwsIdentityTypeDef = ...,
-        subscriberName: str = ...
+        subscriberName: str = ...,
     ) -> UpdateSubscriberResponseTypeDef:
         """
         Updates an existing subscription for the given Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_subscriber)
         """
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/client.pyi` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     async def create_custom_log_source(
         self,
         *,
         sourceName: str,
         configuration: CustomLogSourceConfigurationTypeDef = ...,
         eventClasses: Sequence[str] = ...,
-        sourceVersion: str = ...
+        sourceVersion: str = ...,
     ) -> CreateCustomLogSourceResponseTypeDef:
         """
         Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
         Services Region where you want to create a custom
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
@@ -141,30 +141,30 @@
         """
 
     async def create_data_lake(
         self,
         *,
         configurations: Sequence[DataLakeConfigurationTypeDef],
         metaStoreManagerRoleArn: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake)
         """
 
     async def create_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
-        exceptionTimeToLive: int = ...
+        exceptionTimeToLive: int = ...,
     ) -> Dict[str, Any]:
         """
         Creates the specified notification subscription in Amazon Security Lake for the
         organization you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
@@ -186,15 +186,15 @@
         self,
         *,
         sources: Sequence[LogSourceResourceTypeDef],
         subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
         subscriberDescription: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security
         Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
@@ -385,15 +385,15 @@
     async def list_log_sources(
         self,
         *,
         accounts: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regions: Sequence[str] = ...,
-        sources: Sequence[LogSourceResourceTypeDef] = ...
+        sources: Sequence[LogSourceResourceTypeDef] = ...,
     ) -> ListLogSourcesResponseTypeDef:
         """
         Retrieves the log sources in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_log_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_log_sources)
         """
@@ -463,15 +463,15 @@
         """
 
     async def update_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
-        exceptionTimeToLive: int = ...
+        exceptionTimeToLive: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates the specified notification subscription in Amazon Security Lake for the
         organization you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake_exception_subscription)
@@ -481,15 +481,15 @@
     async def update_subscriber(
         self,
         *,
         subscriberId: str,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
         subscriberDescription: str = ...,
         subscriberIdentity: AwsIdentityTypeDef = ...,
-        subscriberName: str = ...
+        subscriberName: str = ...,
     ) -> UpdateSubscriberResponseTypeDef:
         """
         Updates an existing subscription for the given Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_subscriber)
         """
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/literals.py` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/literals.py`

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
     "AccessTypeType",
     "AwsLogSourceNameType",
     "DataLakeStatusType",
     "GetDataLakeSourcesPaginatorName",
     "HttpMethodType",
     "ListDataLakeExceptionsPaginatorName",
@@ -34,15 +33,14 @@
     "SecurityLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessTypeType = Literal["LAKEFORMATION", "S3"]
 AwsLogSourceNameType = Literal[
     "CLOUD_TRAIL_MGMT", "LAMBDA_EXECUTION", "ROUTE53", "S3_DATA", "SH_FINDINGS", "VPC_FLOW"
 ]
 DataLakeStatusType = Literal["COMPLETED", "FAILED", "INITIALIZED", "PENDING"]
 GetDataLakeSourcesPaginatorName = Literal["get_data_lake_sources"]
 HttpMethodType = Literal["POST", "PUT"]
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/literals.pyi` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/paginator.py` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "GetDataLakeSourcesPaginator",
     "ListDataLakeExceptionsPaginator",
     "ListLogSourcesPaginator",
     "ListSubscribersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -97,15 +96,15 @@
 
     def paginate(
         self,
         *,
         accounts: Sequence[str] = ...,
         regions: Sequence[str] = ...,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listlogsourcespaginator)
         """
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/paginator.pyi` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     def paginate(
         self,
         *,
         accounts: Sequence[str] = ...,
         regions: Sequence[str] = ...,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/paginators/#listlogsourcespaginator)
         """
 
 class ListSubscribersPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/type_defs.py` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
     "AwsLogSourceResourceTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake/type_defs.pyi` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/PKG-INFO` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SecurityLake 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SecurityLake 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
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
 
 <a id="types-aiobotocore-securitylake"></a>
 
 # types-aiobotocore-securitylake
 
 [![PyPI - types-aiobotocore-securitylake](https://img.shields.io/pypi/v/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityLake 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[aiobotocore.SecurityLake 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-securitylake-2.9.0/types_aiobotocore_securitylake.egg-info/SOURCES.txt` & `types-aiobotocore-securitylake-2.9.1/types_aiobotocore_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

