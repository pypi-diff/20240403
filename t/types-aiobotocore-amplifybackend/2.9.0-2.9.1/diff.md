# Comparing `tmp/types-aiobotocore-amplifybackend-2.9.0.tar.gz` & `tmp/types-aiobotocore-amplifybackend-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplifybackend-2.9.0.tar", last modified: Wed Dec 13 19:58:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplifybackend-2.9.1.tar", last modified: Thu Jan 18 01:19:59 2024, max compression
```

## Comparing `types-aiobotocore-amplifybackend-2.9.0.tar` & `types-aiobotocore-amplifybackend-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:31.250124 types-aiobotocore-amplifybackend-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2023-12-13 19:58:31.246124 types-aiobotocore-amplifybackend-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:31.250124 types-aiobotocore-amplifybackend-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:31.246124 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24804 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24800 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31448 2023-12-13 19:40:45.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31447 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:44.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:31.246124 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2023-12-13 19:58:31.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:58:31.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:31.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:31.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:31.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:58:31.000000 types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:59.637530 types-aiobotocore-amplifybackend-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-01-18 01:19:59.637530 types-aiobotocore-amplifybackend-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:59.637530 types-aiobotocore-amplifybackend-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:59.633530 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24817 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24814 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-01-18 01:02:44.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-01-18 01:02:44.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    31447 2024-01-18 01:02:44.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31447 2024-01-18 01:02:44.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:43.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:59.637530 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-01-18 01:19:59.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:19:59.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:59.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:59.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:59.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:19:59.000000 types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/LICENSE` & `types-aiobotocore-amplifybackend-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-amplifybackend-2.9.0/PKG-INFO` & `types-aiobotocore-amplifybackend-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifybackend
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AmplifyBackend 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AmplifyBackend 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/
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
 
 <a id="types-aiobotocore-amplifybackend"></a>
 
 # types-aiobotocore-amplifybackend
 
 [![PyPI - types-aiobotocore-amplifybackend](https://img.shields.io/pypi/v/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifybackend)](https://pepy.tech/project/types-aiobotocore-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AmplifyBackend 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[aiobotocore.AmplifyBackend 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [types-aiobotocore-amplifybackend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/README.md` & `types-aiobotocore-amplifybackend-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifybackend)](https://pepy.tech/project/types-aiobotocore-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AmplifyBackend 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[aiobotocore.AmplifyBackend 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [types-aiobotocore-amplifybackend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/setup.py` & `types-aiobotocore-amplifybackend-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplifybackend",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AmplifyBackend 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AmplifyBackend 2.9.1 service generated with"
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
     keywords="aiobotocore amplifybackend type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_amplifybackend": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/__init__.py` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import AmplifyBackendClient
 from .paginator import ListBackendJobsPaginator
 
 Client = AmplifyBackendClient
 
-
 __all__ = ("AmplifyBackendClient", "Client", "ListBackendJobsPaginator")
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/__init__.pyi` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/__main__.py` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AmplifyBackend 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AmplifyBackend 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
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

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/client.py` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AmplifyBackendClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -133,45 +132,45 @@
     async def create_backend(
         self,
         *,
         AppId: str,
         AppName: str,
         BackendEnvironmentName: str,
         ResourceConfig: Mapping[str, Any] = ...,
-        ResourceName: str = ...
+        ResourceName: str = ...,
     ) -> CreateBackendResponseTypeDef:
         """
         This operation creates a backend for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend)
         """
 
     async def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: BackendAPIResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_api)
         """
 
     async def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_auth)
         """
@@ -188,15 +187,15 @@
 
     async def create_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: CreateBackendStorageResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> CreateBackendStorageResponseTypeDef:
         """
         Creates a backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_storage)
         """
@@ -223,15 +222,15 @@
 
     async def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...,
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_api)
         """
@@ -248,15 +247,15 @@
 
     async def delete_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ServiceName: Literal["S3"]
+        ServiceName: Literal["S3"],
     ) -> DeleteBackendStorageResponseTypeDef:
         """
         Removes the specified backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_storage)
         """
@@ -305,15 +304,15 @@
 
     async def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...,
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#get_backend_api)
         """
@@ -370,30 +369,30 @@
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         NativeClientId: str,
         UserPoolId: str,
         WebClientId: str,
-        IdentityPoolId: str = ...
+        IdentityPoolId: str = ...,
     ) -> ImportBackendAuthResponseTypeDef:
         """
         Imports an existing backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.import_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#import_backend_auth)
         """
 
     async def import_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ServiceName: Literal["S3"],
-        BucketName: str = ...
+        BucketName: str = ...,
     ) -> ImportBackendStorageResponseTypeDef:
         """
         Imports an existing backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.import_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#import_backend_storage)
         """
@@ -403,15 +402,15 @@
         *,
         AppId: str,
         BackendEnvironmentName: str,
         JobId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Operation: str = ...,
-        Status: str = ...
+        Status: str = ...,
     ) -> ListBackendJobsResponseTypeDef:
         """
         Lists the jobs for the backend of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.list_backend_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#list_backend_jobs)
         """
@@ -444,30 +443,30 @@
 
     async def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...,
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_api)
         """
 
     async def update_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: UpdateBackendAuthResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> UpdateBackendAuthResponseTypeDef:
         """
         Updates an existing backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_auth)
         """
@@ -485,30 +484,30 @@
     async def update_backend_job(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         JobId: str,
         Operation: str = ...,
-        Status: str = ...
+        Status: str = ...,
     ) -> UpdateBackendJobResponseTypeDef:
         """
         Updates a specific job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_job)
         """
 
     async def update_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: UpdateBackendStorageResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> UpdateBackendStorageResponseTypeDef:
         """
         Updates an existing backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_storage)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/client.pyi` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -129,45 +129,45 @@
     async def create_backend(
         self,
         *,
         AppId: str,
         AppName: str,
         BackendEnvironmentName: str,
         ResourceConfig: Mapping[str, Any] = ...,
-        ResourceName: str = ...
+        ResourceName: str = ...,
     ) -> CreateBackendResponseTypeDef:
         """
         This operation creates a backend for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend)
         """
 
     async def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: BackendAPIResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_api)
         """
 
     async def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_auth)
         """
@@ -184,15 +184,15 @@
 
     async def create_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: CreateBackendStorageResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> CreateBackendStorageResponseTypeDef:
         """
         Creates a backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_storage)
         """
@@ -219,15 +219,15 @@
 
     async def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...,
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_api)
         """
@@ -244,15 +244,15 @@
 
     async def delete_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ServiceName: Literal["S3"]
+        ServiceName: Literal["S3"],
     ) -> DeleteBackendStorageResponseTypeDef:
         """
         Removes the specified backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_storage)
         """
@@ -301,15 +301,15 @@
 
     async def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...,
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#get_backend_api)
         """
@@ -366,30 +366,30 @@
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         NativeClientId: str,
         UserPoolId: str,
         WebClientId: str,
-        IdentityPoolId: str = ...
+        IdentityPoolId: str = ...,
     ) -> ImportBackendAuthResponseTypeDef:
         """
         Imports an existing backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.import_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#import_backend_auth)
         """
 
     async def import_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ServiceName: Literal["S3"],
-        BucketName: str = ...
+        BucketName: str = ...,
     ) -> ImportBackendStorageResponseTypeDef:
         """
         Imports an existing backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.import_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#import_backend_storage)
         """
@@ -399,15 +399,15 @@
         *,
         AppId: str,
         BackendEnvironmentName: str,
         JobId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Operation: str = ...,
-        Status: str = ...
+        Status: str = ...,
     ) -> ListBackendJobsResponseTypeDef:
         """
         Lists the jobs for the backend of an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.list_backend_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#list_backend_jobs)
         """
@@ -440,30 +440,30 @@
 
     async def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...,
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_api)
         """
 
     async def update_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: UpdateBackendAuthResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> UpdateBackendAuthResponseTypeDef:
         """
         Updates an existing backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_auth)
         """
@@ -481,30 +481,30 @@
     async def update_backend_job(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         JobId: str,
         Operation: str = ...,
-        Status: str = ...
+        Status: str = ...,
     ) -> UpdateBackendJobResponseTypeDef:
         """
         Updates a specific job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_job)
         """
 
     async def update_backend_storage(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceConfig: UpdateBackendStorageResourceConfigTypeDef,
-        ResourceName: str
+        ResourceName: str,
     ) -> UpdateBackendStorageResponseTypeDef:
         """
         Updates an existing backend storage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_storage)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/literals.py` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/literals.py`

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
     "AdditionalConstraintsElementType",
     "AuthResourcesType",
     "AuthenticatedElementType",
     "DeliveryMethodType",
     "ListBackendJobsPaginatorName",
     "MFAModeType",
@@ -41,15 +40,14 @@
     "AmplifyBackendServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdditionalConstraintsElementType = Literal[
     "REQUIRE_DIGIT", "REQUIRE_LOWERCASE", "REQUIRE_SYMBOL", "REQUIRE_UPPERCASE"
 ]
 AuthResourcesType = Literal["IDENTITY_POOL_AND_USER_POOL", "USER_POOL_ONLY"]
 AuthenticatedElementType = Literal["CREATE_AND_UPDATE", "DELETE", "READ"]
 DeliveryMethodType = Literal["EMAIL", "SMS"]
 ListBackendJobsPaginatorName = Literal["list_backend_jobs"]
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/literals.pyi` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/paginator.py` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListBackendJobsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListBackendJobsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -51,13 +50,13 @@
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         JobId: str = ...,
         Operation: str = ...,
         Status: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackendJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Paginator.ListBackendJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/paginators/#listbackendjobspaginator)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/paginator.pyi` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,13 +48,13 @@
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         JobId: str = ...,
         Operation: str = ...,
         Status: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBackendJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Paginator.ListBackendJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/paginators/#listbackendjobspaginator)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/type_defs.py` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BackendAPIAppSyncAuthSettingsTypeDef",
     "BackendAPIConflictResolutionTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
     "BackendStoragePermissionsTypeDef",
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend/type_defs.pyi` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/PKG-INFO` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifybackend
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AmplifyBackend 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AmplifyBackend 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/
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
 
 <a id="types-aiobotocore-amplifybackend"></a>
 
 # types-aiobotocore-amplifybackend
 
 [![PyPI - types-aiobotocore-amplifybackend](https://img.shields.io/pypi/v/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifybackend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifybackend)](https://pepy.tech/project/types-aiobotocore-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AmplifyBackend 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[aiobotocore.AmplifyBackend 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [types-aiobotocore-amplifybackend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-amplifybackend-2.9.0/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt` & `types-aiobotocore-amplifybackend-2.9.1/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

