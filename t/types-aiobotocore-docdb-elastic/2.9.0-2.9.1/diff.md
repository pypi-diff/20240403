# Comparing `tmp/types-aiobotocore-docdb-elastic-2.9.0.tar.gz` & `tmp/types-aiobotocore-docdb-elastic-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-elastic-2.9.0.tar", last modified: Wed Dec 13 19:59:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-elastic-2.9.1.tar", last modified: Thu Jan 18 01:20:33 2024, max compression
```

## Comparing `types-aiobotocore-docdb-elastic-2.9.0.tar` & `types-aiobotocore-docdb-elastic-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.957822 types-aiobotocore-docdb-elastic-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2023-12-13 19:59:07.957822 types-aiobotocore-docdb-elastic-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:07.957822 types-aiobotocore-docdb-elastic-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.957822 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14196 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8718 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2023-12-13 19:44:23.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.957822 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2023-12-13 19:59:07.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:59:07.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:07.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:07.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:07.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:07.000000 types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.253379 types-aiobotocore-docdb-elastic-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-01-18 01:20:33.253379 types-aiobotocore-docdb-elastic-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:33.253379 types-aiobotocore-docdb-elastic-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.253379 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.253379 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/LICENSE` & `types-aiobotocore-docdb-elastic-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DocDBElastic 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DocDBElastic 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
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
 
 <a id="types-aiobotocore-docdb-elastic"></a>
 
 # types-aiobotocore-docdb-elastic
 
 [![PyPI - types-aiobotocore-docdb-elastic](https://img.shields.io/pypi/v/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb-elastic)](https://pepy.tech/project/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDBElastic 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[aiobotocore.DocDBElastic 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/README.md` & `types-aiobotocore-docdb-elastic-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb-elastic)](https://pepy.tech/project/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDBElastic 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[aiobotocore.DocDBElastic 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/setup.py` & `types-aiobotocore-docdb-elastic-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb-elastic",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_docdb_elastic"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DocDBElastic 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DocDBElastic 2.9.1 service generated with"
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
     keywords="aiobotocore docdb-elastic type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_docdb_elastic": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/__init__.py` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import DocDBElasticClient
 from .paginator import ListClusterSnapshotsPaginator, ListClustersPaginator
 
 Client = DocDBElasticClient
 
-
 __all__ = ("Client", "DocDBElasticClient", "ListClusterSnapshotsPaginator", "ListClustersPaginator")
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/__init__.pyi` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/__main__.py` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DocDBElastic 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DocDBElastic 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic\nOther"
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

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/client.py` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DocDBElasticClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -108,15 +107,15 @@
         shardCapacity: int,
         shardCount: int,
         clientToken: str = ...,
         kmsKeyId: str = ...,
         preferredMaintenanceWindow: str = ...,
         subnetIds: Sequence[str] = ...,
         tags: Mapping[str, str] = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> CreateClusterOutputTypeDef:
         """
         Creates a new Elastic DocumentDB cluster and returns its Cluster structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/client/#create_cluster)
         """
@@ -216,15 +215,15 @@
         self,
         *,
         clusterName: str,
         snapshotArn: str,
         kmsKeyId: str = ...,
         subnetIds: Sequence[str] = ...,
         tags: Mapping[str, str] = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> RestoreClusterFromSnapshotOutputTypeDef:
         """
         Restores a Elastic DocumentDB cluster from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.restore_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/client/#restore_cluster_from_snapshot)
         """
@@ -254,15 +253,15 @@
         adminUserPassword: str = ...,
         authType: AuthType = ...,
         clientToken: str = ...,
         preferredMaintenanceWindow: str = ...,
         shardCapacity: int = ...,
         shardCount: int = ...,
         subnetIds: Sequence[str] = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> UpdateClusterOutputTypeDef:
         """
         Modifies a Elastic DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/client/#update_cluster)
         """
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/client.pyi` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         shardCapacity: int,
         shardCount: int,
         clientToken: str = ...,
         kmsKeyId: str = ...,
         preferredMaintenanceWindow: str = ...,
         subnetIds: Sequence[str] = ...,
         tags: Mapping[str, str] = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> CreateClusterOutputTypeDef:
         """
         Creates a new Elastic DocumentDB cluster and returns its Cluster structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/client/#create_cluster)
         """
@@ -212,15 +212,15 @@
         self,
         *,
         clusterName: str,
         snapshotArn: str,
         kmsKeyId: str = ...,
         subnetIds: Sequence[str] = ...,
         tags: Mapping[str, str] = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> RestoreClusterFromSnapshotOutputTypeDef:
         """
         Restores a Elastic DocumentDB cluster from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.restore_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/client/#restore_cluster_from_snapshot)
         """
@@ -250,15 +250,15 @@
         adminUserPassword: str = ...,
         authType: AuthType = ...,
         clientToken: str = ...,
         preferredMaintenanceWindow: str = ...,
         shardCapacity: int = ...,
         shardCount: int = ...,
         subnetIds: Sequence[str] = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> UpdateClusterOutputTypeDef:
         """
         Modifies a Elastic DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/client/#update_cluster)
         """
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/literals.py` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthType",
     "ListClusterSnapshotsPaginatorName",
     "ListClustersPaginatorName",
     "StatusType",
     "DocDBElasticServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AuthType = Literal["PLAIN_TEXT", "SECRET_ARN"]
 ListClusterSnapshotsPaginatorName = Literal["list_cluster_snapshots"]
 ListClustersPaginatorName = Literal["list_clusters"]
 StatusType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETING",
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/literals.pyi` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/paginator.py` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListClusterSnapshotsOutputTypeDef,
     ListClustersOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListClusterSnapshotsPaginator", "ListClustersPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/paginator.pyi` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/type_defs.py` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic/type_defs.pyi` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DocDBElastic 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DocDBElastic 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
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
 
 <a id="types-aiobotocore-docdb-elastic"></a>
 
 # types-aiobotocore-docdb-elastic
 
 [![PyPI - types-aiobotocore-docdb-elastic](https://img.shields.io/pypi/v/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb-elastic.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb-elastic)](https://pepy.tech/project/types-aiobotocore-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDBElastic 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[aiobotocore.DocDBElastic 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-docdb-elastic-2.9.0/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-elastic-2.9.1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

