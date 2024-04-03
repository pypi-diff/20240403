# Comparing `tmp/types-aiobotocore-secretsmanager-2.9.0.tar.gz` & `tmp/types-aiobotocore-secretsmanager-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-secretsmanager-2.9.0.tar", last modified: Wed Dec 13 20:00:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-secretsmanager-2.9.1.tar", last modified: Thu Jan 18 01:21:46 2024, max compression
```

## Comparing `types-aiobotocore-secretsmanager-2.9.0.tar` & `types-aiobotocore-secretsmanager-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:27.945159 types-aiobotocore-secretsmanager-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2023-12-13 20:00:27.945159 types-aiobotocore-secretsmanager-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:27.945159 types-aiobotocore-secretsmanager-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:27.945159 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21120 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2023-12-13 19:55:52.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18297 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:51.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:27.945159 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2023-12-13 20:00:27.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:27.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:27.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:27.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:27.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:27.000000 types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:46.585044 types-aiobotocore-secretsmanager-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-01-18 01:21:46.585044 types-aiobotocore-secretsmanager-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:46.585044 types-aiobotocore-secretsmanager-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:46.585044 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21130 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21127 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18297 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18297 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:22.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:46.585044 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-01-18 01:21:46.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:46.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:46.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:46.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:46.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:46.000000 types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/LICENSE` & `types-aiobotocore-secretsmanager-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-secretsmanager-2.9.0/PKG-INFO` & `types-aiobotocore-secretsmanager-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SecretsManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SecretsManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
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
 
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecretsManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[aiobotocore.SecretsManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/README.md` & `types-aiobotocore-secretsmanager-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecretsManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[aiobotocore.SecretsManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/setup.py` & `types-aiobotocore-secretsmanager-2.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-secretsmanager",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SecretsManager 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SecretsManager 2.9.1 service generated with"
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
     keywords="aiobotocore secretsmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_secretsmanager": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/__init__.py` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import SecretsManagerClient
 from .paginator import ListSecretsPaginator
 
 Client = SecretsManagerClient
 
-
 __all__ = ("Client", "ListSecretsPaginator", "SecretsManagerClient")
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/__init__.pyi` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/__main__.py` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecretsManager 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SecretsManager 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/client.py` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SecretsManagerClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DecryptionFailure: Type[BotocoreClientError]
     EncryptionFailure: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -81,15 +78,14 @@
     LimitExceededException: Type[BotocoreClientError]
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     PreconditionNotMetException: Type[BotocoreClientError]
     PublicPolicyException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
-
 class SecretsManagerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/)
     """
 
     meta: ClientMeta
@@ -105,15 +101,15 @@
 
     async def batch_get_secret_value(
         self,
         *,
         SecretIdList: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> BatchGetSecretValueResponseTypeDef:
         """
         Retrieves the contents of the encrypted fields `SecretString` or `SecretBinary`
         for up to 20
         secrets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.batch_get_secret_value)
@@ -153,15 +149,15 @@
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
-        ForceOverwriteReplicaSecret: bool = ...
+        ForceOverwriteReplicaSecret: bool = ...,
     ) -> CreateSecretResponseTypeDef:
         """
         Creates a new secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.create_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#create_secret)
         """
@@ -175,15 +171,15 @@
         """
 
     async def delete_secret(
         self,
         *,
         SecretId: str,
         RecoveryWindowInDays: int = ...,
-        ForceDeleteWithoutRecovery: bool = ...
+        ForceDeleteWithoutRecovery: bool = ...,
     ) -> DeleteSecretResponseTypeDef:
         """
         Deletes a secret and all of its versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#delete_secret)
         """
@@ -216,15 +212,15 @@
         PasswordLength: int = ...,
         ExcludeCharacters: str = ...,
         ExcludeNumbers: bool = ...,
         ExcludePunctuation: bool = ...,
         ExcludeUppercase: bool = ...,
         ExcludeLowercase: bool = ...,
         IncludeSpace: bool = ...,
-        RequireEachIncludedType: bool = ...
+        RequireEachIncludedType: bool = ...,
     ) -> GetRandomPasswordResponseTypeDef:
         """
         Generates a random password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_random_password)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#get_random_password)
         """
@@ -252,15 +248,15 @@
 
     async def list_secret_version_ids(
         self,
         *,
         SecretId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        IncludeDeprecated: bool = ...
+        IncludeDeprecated: bool = ...,
     ) -> ListSecretVersionIdsResponseTypeDef:
         """
         Lists the versions of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secret_version_ids)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#list_secret_version_ids)
         """
@@ -268,15 +264,15 @@
     async def list_secrets(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortOrder: SortOrderTypeType = ...
+        SortOrder: SortOrderTypeType = ...,
     ) -> ListSecretsResponseTypeDef:
         """
         Lists the secrets that are stored by Secrets Manager in the Amazon Web Services
         account, not including secrets that are marked for
         deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secrets)
@@ -296,15 +292,15 @@
     async def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
-        VersionStages: Sequence[str] = ...
+        VersionStages: Sequence[str] = ...,
     ) -> PutSecretValueResponseTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_secret_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#put_secret_value)
@@ -323,15 +319,15 @@
         """
 
     async def replicate_secret_to_regions(
         self,
         *,
         SecretId: str,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],
-        ForceOverwriteReplicaSecret: bool = ...
+        ForceOverwriteReplicaSecret: bool = ...,
     ) -> ReplicateSecretToRegionsResponseTypeDef:
         """
         Replicates the secret to a new Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.replicate_secret_to_regions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#replicate_secret_to_regions)
         """
@@ -348,15 +344,15 @@
     async def rotate_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         RotationLambdaARN: str = ...,
         RotationRules: RotationRulesTypeTypeDef = ...,
-        RotateImmediately: bool = ...
+        RotateImmediately: bool = ...,
     ) -> RotateSecretResponseTypeDef:
         """
         Configures and starts the asynchronous process of rotating the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.rotate_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#rotate_secret)
         """
@@ -397,30 +393,30 @@
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: BlobTypeDef = ...,
-        SecretString: str = ...
+        SecretString: str = ...,
     ) -> UpdateSecretResponseTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#update_secret)
         """
 
     async def update_secret_version_stage(
         self,
         *,
         SecretId: str,
         VersionStage: str,
         RemoveFromVersionId: str = ...,
-        MoveToVersionId: str = ...
+        MoveToVersionId: str = ...,
     ) -> UpdateSecretVersionStageResponseTypeDef:
         """
         Modifies the staging labels attached to a version of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret_version_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#update_secret_version_stage)
         """
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/client.pyi` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("SecretsManagerClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DecryptionFailure: Type[BotocoreClientError]
     EncryptionFailure: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -78,14 +80,15 @@
     LimitExceededException: Type[BotocoreClientError]
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     PreconditionNotMetException: Type[BotocoreClientError]
     PublicPolicyException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
 
+
 class SecretsManagerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/)
     """
 
     meta: ClientMeta
@@ -101,15 +104,15 @@
 
     async def batch_get_secret_value(
         self,
         *,
         SecretIdList: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> BatchGetSecretValueResponseTypeDef:
         """
         Retrieves the contents of the encrypted fields `SecretString` or `SecretBinary`
         for up to 20
         secrets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.batch_get_secret_value)
@@ -149,15 +152,15 @@
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
-        ForceOverwriteReplicaSecret: bool = ...
+        ForceOverwriteReplicaSecret: bool = ...,
     ) -> CreateSecretResponseTypeDef:
         """
         Creates a new secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.create_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#create_secret)
         """
@@ -171,15 +174,15 @@
         """
 
     async def delete_secret(
         self,
         *,
         SecretId: str,
         RecoveryWindowInDays: int = ...,
-        ForceDeleteWithoutRecovery: bool = ...
+        ForceDeleteWithoutRecovery: bool = ...,
     ) -> DeleteSecretResponseTypeDef:
         """
         Deletes a secret and all of its versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.delete_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#delete_secret)
         """
@@ -212,15 +215,15 @@
         PasswordLength: int = ...,
         ExcludeCharacters: str = ...,
         ExcludeNumbers: bool = ...,
         ExcludePunctuation: bool = ...,
         ExcludeUppercase: bool = ...,
         ExcludeLowercase: bool = ...,
         IncludeSpace: bool = ...,
-        RequireEachIncludedType: bool = ...
+        RequireEachIncludedType: bool = ...,
     ) -> GetRandomPasswordResponseTypeDef:
         """
         Generates a random password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.get_random_password)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#get_random_password)
         """
@@ -248,15 +251,15 @@
 
     async def list_secret_version_ids(
         self,
         *,
         SecretId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        IncludeDeprecated: bool = ...
+        IncludeDeprecated: bool = ...,
     ) -> ListSecretVersionIdsResponseTypeDef:
         """
         Lists the versions of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secret_version_ids)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#list_secret_version_ids)
         """
@@ -264,15 +267,15 @@
     async def list_secrets(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        SortOrder: SortOrderTypeType = ...
+        SortOrder: SortOrderTypeType = ...,
     ) -> ListSecretsResponseTypeDef:
         """
         Lists the secrets that are stored by Secrets Manager in the Amazon Web Services
         account, not including secrets that are marked for
         deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.list_secrets)
@@ -292,15 +295,15 @@
     async def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
-        VersionStages: Sequence[str] = ...
+        VersionStages: Sequence[str] = ...,
     ) -> PutSecretValueResponseTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.put_secret_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#put_secret_value)
@@ -319,15 +322,15 @@
         """
 
     async def replicate_secret_to_regions(
         self,
         *,
         SecretId: str,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],
-        ForceOverwriteReplicaSecret: bool = ...
+        ForceOverwriteReplicaSecret: bool = ...,
     ) -> ReplicateSecretToRegionsResponseTypeDef:
         """
         Replicates the secret to a new Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.replicate_secret_to_regions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#replicate_secret_to_regions)
         """
@@ -344,15 +347,15 @@
     async def rotate_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         RotationLambdaARN: str = ...,
         RotationRules: RotationRulesTypeTypeDef = ...,
-        RotateImmediately: bool = ...
+        RotateImmediately: bool = ...,
     ) -> RotateSecretResponseTypeDef:
         """
         Configures and starts the asynchronous process of rotating the secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.rotate_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#rotate_secret)
         """
@@ -393,30 +396,30 @@
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
         SecretBinary: BlobTypeDef = ...,
-        SecretString: str = ...
+        SecretString: str = ...,
     ) -> UpdateSecretResponseTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#update_secret)
         """
 
     async def update_secret_version_stage(
         self,
         *,
         SecretId: str,
         VersionStage: str,
         RemoveFromVersionId: str = ...,
-        MoveToVersionId: str = ...
+        MoveToVersionId: str = ...,
     ) -> UpdateSecretVersionStageResponseTypeDef:
         """
         Modifies the staging labels attached to a version of a secret.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret_version_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#update_secret_version_stage)
         """
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/literals.py` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "FilterNameStringTypeType",
     "ListSecretsPaginatorName",
     "SortOrderTypeType",
     "StatusTypeType",
     "SecretsManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 FilterNameStringTypeType = Literal[
     "all", "description", "name", "owning-service", "primary-region", "tag-key", "tag-value"
 ]
 ListSecretsPaginatorName = Literal["list_secrets"]
 SortOrderTypeType = Literal["asc", "desc"]
 StatusTypeType = Literal["Failed", "InProgress", "InSync"]
 SecretsManagerServiceName = Literal["secretsmanager"]
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/literals.pyi` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/paginator.py` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import SortOrderTypeType
 from .type_defs import FilterTypeDef, ListSecretsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListSecretsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -50,13 +49,13 @@
 
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/paginator.pyi` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/type_defs.py` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "APIErrorTypeTypeDef",
     "FilterTypeDef",
     "ResponseMetadataTypeDef",
     "SecretValueEntryTypeDef",
     "BlobTypeDef",
     "CancelRotateSecretRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager/type_defs.pyi` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/PKG-INFO` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SecretsManager 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SecretsManager 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
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
 
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecretsManager 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[aiobotocore.SecretsManager 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-secretsmanager-2.9.0/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt` & `types-aiobotocore-secretsmanager-2.9.1/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

