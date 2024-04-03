# Comparing `tmp/types-aiobotocore-lookoutvision-2.9.0.tar.gz` & `tmp/types-aiobotocore-lookoutvision-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutvision-2.9.0.tar", last modified: Wed Dec 13 19:59:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutvision-2.9.1.tar", last modified: Thu Jan 18 01:21:10 2024, max compression
```

## Comparing `types-aiobotocore-lookoutvision-2.9.0.tar` & `types-aiobotocore-lookoutvision-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.221506 types-aiobotocore-lookoutvision-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2023-12-13 19:59:48.221506 types-aiobotocore-lookoutvision-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:48.221506 types-aiobotocore-lookoutvision-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.221506 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20431 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2023-12-13 19:49:31.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21323 2023-12-13 19:49:33.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2023-12-13 19:49:31.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:30.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.221506 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2023-12-13 19:59:48.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:59:48.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:48.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:48.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:48.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:48.000000 types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.505207 types-aiobotocore-lookoutvision-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-01-18 01:21:10.505207 types-aiobotocore-lookoutvision-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:10.505207 types-aiobotocore-lookoutvision-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.501207 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20439 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:17.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:10.501207 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:10.000000 types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/LICENSE` & `types-aiobotocore-lookoutvision-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lookoutvision-2.9.0/PKG-INFO` & `types-aiobotocore-lookoutvision-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutvision
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LookoutforVision 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LookoutforVision 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/
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
 
 <a id="types-aiobotocore-lookoutvision"></a>
 
 # types-aiobotocore-lookoutvision
 
 [![PyPI - types-aiobotocore-lookoutvision](https://img.shields.io/pypi/v/types-aiobotocore-lookoutvision.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutvision.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutvision)](https://pepy.tech/project/types-aiobotocore-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutforVision 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[aiobotocore.LookoutforVision 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [types-aiobotocore-lookoutvision docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/README.md` & `types-aiobotocore-lookoutvision-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutvision.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutvision)](https://pepy.tech/project/types-aiobotocore-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutforVision 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[aiobotocore.LookoutforVision 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [types-aiobotocore-lookoutvision docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/setup.py` & `types-aiobotocore-lookoutvision-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutvision",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LookoutforVision 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LookoutforVision 2.9.1 service generated with"
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
     keywords="aiobotocore lookoutvision type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lookoutvision": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/__init__.py` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListModelPackagingJobsPaginator,
     ListModelsPaginator,
     ListProjectsPaginator,
 )
 
 Client = LookoutforVisionClient
 
-
 __all__ = (
     "Client",
     "ListDatasetEntriesPaginator",
     "ListModelPackagingJobsPaginator",
     "ListModelsPaginator",
     "ListProjectsPaginator",
     "LookoutforVisionClient",
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/__init__.pyi` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/__main__.py` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LookoutforVision 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LookoutforVision 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision\nOther"
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

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/client.py` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LookoutforVisionClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -118,15 +117,15 @@
 
     async def create_dataset(
         self,
         *,
         ProjectName: str,
         DatasetType: str,
         DatasetSource: DatasetSourceTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new dataset in an Amazon Lookout for Vision project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#create_dataset)
         """
@@ -135,15 +134,15 @@
         self,
         *,
         ProjectName: str,
         OutputConfig: OutputConfigTypeDef,
         Description: str = ...,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelResponseTypeDef:
         """
         Creates a new version of a model within an an Amazon Lookout for Vision project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#create_model)
         """
@@ -257,15 +256,15 @@
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: TimestampTypeDef = ...,
         AfterCreationDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SourceRefContains: str = ...
+        SourceRefContains: str = ...,
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         Lists the JSON Lines within a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#list_dataset_entries)
         """
@@ -316,15 +315,15 @@
     async def start_model(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
         MinInferenceUnits: int,
         ClientToken: str = ...,
-        MaxInferenceUnits: int = ...
+        MaxInferenceUnits: int = ...,
     ) -> StartModelResponseTypeDef:
         """
         Starts the running of the version of an Amazon Lookout for Vision model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.start_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#start_model)
         """
@@ -333,15 +332,15 @@
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
         Configuration: ModelPackagingConfigurationTypeDef,
         JobName: str = ...,
         Description: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.start_model_packaging_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#start_model_packaging_job)
         """
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/client.pyi` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     async def create_dataset(
         self,
         *,
         ProjectName: str,
         DatasetType: str,
         DatasetSource: DatasetSourceTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new dataset in an Amazon Lookout for Vision project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#create_dataset)
         """
@@ -131,15 +131,15 @@
         self,
         *,
         ProjectName: str,
         OutputConfig: OutputConfigTypeDef,
         Description: str = ...,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelResponseTypeDef:
         """
         Creates a new version of a model within an an Amazon Lookout for Vision project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#create_model)
         """
@@ -253,15 +253,15 @@
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: TimestampTypeDef = ...,
         AfterCreationDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SourceRefContains: str = ...
+        SourceRefContains: str = ...,
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         Lists the JSON Lines within a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#list_dataset_entries)
         """
@@ -312,15 +312,15 @@
     async def start_model(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
         MinInferenceUnits: int,
         ClientToken: str = ...,
-        MaxInferenceUnits: int = ...
+        MaxInferenceUnits: int = ...,
     ) -> StartModelResponseTypeDef:
         """
         Starts the running of the version of an Amazon Lookout for Vision model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.start_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#start_model)
         """
@@ -329,15 +329,15 @@
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
         Configuration: ModelPackagingConfigurationTypeDef,
         JobName: str = ...,
         Description: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.start_model_packaging_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#start_model_packaging_job)
         """
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/literals.py` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/literals.py`

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
     "DatasetStatusType",
     "ListDatasetEntriesPaginatorName",
     "ListModelPackagingJobsPaginatorName",
     "ListModelsPaginatorName",
     "ListProjectsPaginatorName",
     "ModelHostingStatusType",
@@ -36,15 +35,14 @@
     "LookoutforVisionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DatasetStatusType = Literal[
     "CREATE_COMPLETE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/literals.pyi` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/paginator.py` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "ListDatasetEntriesPaginator",
     "ListModelPackagingJobsPaginator",
     "ListModelsPaginator",
     "ListProjectsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -71,15 +70,15 @@
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: TimestampTypeDef = ...,
         AfterCreationDate: TimestampTypeDef = ...,
         SourceRefContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/paginators/#listdatasetentriespaginator)
         """
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/paginator.pyi` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: TimestampTypeDef = ...,
         AfterCreationDate: TimestampTypeDef = ...,
         SourceRefContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/paginators/#listdatasetentriespaginator)
         """
 
 class ListModelPackagingJobsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/type_defs.py` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PixelAnomalyTypeDef",
     "BlobTypeDef",
     "DatasetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision/type_defs.pyi` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/PKG-INFO` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutvision
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LookoutforVision 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LookoutforVision 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/
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
 
 <a id="types-aiobotocore-lookoutvision"></a>
 
 # types-aiobotocore-lookoutvision
 
 [![PyPI - types-aiobotocore-lookoutvision](https://img.shields.io/pypi/v/types-aiobotocore-lookoutvision.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutvision.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutvision)](https://pepy.tech/project/types-aiobotocore-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LookoutforVision 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[aiobotocore.LookoutforVision 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [types-aiobotocore-lookoutvision docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lookoutvision-2.9.0/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutvision-2.9.1/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

