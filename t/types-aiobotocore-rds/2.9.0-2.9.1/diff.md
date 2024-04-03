# Comparing `tmp/types-aiobotocore-rds-2.9.0.tar.gz` & `tmp/types-aiobotocore-rds-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rds-2.9.0.tar", last modified: Wed Dec 13 20:00:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-rds-2.9.1.tar", last modified: Thu Jan 18 01:21:35 2024, max compression
```

## Comparing `types-aiobotocore-rds-2.9.0.tar` & `types-aiobotocore-rds-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.437268 types-aiobotocore-rds-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22155 2023-12-13 20:00:15.437268 types-aiobotocore-rds-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20608 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:15.437268 types-aiobotocore-rds-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.433268 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12930 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   162606 2023-12-13 19:54:10.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   162602 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19796 2023-12-13 19:54:13.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    19794 2023-12-13 19:54:10.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    52292 2023-12-13 19:54:10.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    52251 2023-12-13 19:54:10.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   195339 2023-12-13 19:54:17.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   195338 2023-12-13 19:54:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:09.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2023-12-13 19:54:10.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2023-12-13 19:54:10.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.437268 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22155 2023-12-13 20:00:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 20:00:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:15.000000 types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.201095 types-aiobotocore-rds-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22175 2024-01-18 01:21:35.201095 types-aiobotocore-rds-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20608 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:35.201095 types-aiobotocore-rds-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.201095 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/
+-rw-r--r--   0 runner    (1001) docker     (127)    12930 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12930 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162705 2024-01-18 01:15:46.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162702 2024-01-18 01:15:46.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19794 2024-01-18 01:15:47.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19794 2024-01-18 01:15:47.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    52330 2024-01-18 01:15:47.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52290 2024-01-18 01:15:47.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   195338 2024-01-18 01:15:54.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195338 2024-01-18 01:15:53.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:15:45.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-01-18 01:15:47.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-01-18 01:15:47.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.201095 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22175 2024-01-18 01:21:35.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:21:35.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:35.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:35.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:35.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:35.000000 types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rds-2.9.0/LICENSE` & `types-aiobotocore-rds-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-rds-2.9.0/PKG-INFO` & `types-aiobotocore-rds-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RDS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RDS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/
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
 
 <a id="types-aiobotocore-rds"></a>
 
 # types-aiobotocore-rds
 
 [![PyPI - types-aiobotocore-rds](https://img.shields.io/pypi/v/types-aiobotocore-rds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rds)](https://pepy.tech/project/types-aiobotocore-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[aiobotocore.RDS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [types-aiobotocore-rds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rds-2.9.0/README.md` & `types-aiobotocore-rds-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rds)](https://pepy.tech/project/types-aiobotocore-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[aiobotocore.RDS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [types-aiobotocore-rds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rds-2.9.0/setup.py` & `types-aiobotocore-rds-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rds",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RDS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.RDS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore rds type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rds": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/__init__.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,14 @@
     DBSnapshotDeletedWaiter,
     TenantDatabaseAvailableWaiter,
     TenantDatabaseDeletedWaiter,
 )
 
 Client = RDSClient
 
-
 __all__ = (
     "Client",
     "DBClusterAvailableWaiter",
     "DBClusterDeletedWaiter",
     "DBClusterSnapshotAvailableWaiter",
     "DBClusterSnapshotDeletedWaiter",
     "DBInstanceAvailableWaiter",
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/__init__.pyi` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/__main__.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RDS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RDS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\nOther"
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

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/client.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RDSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -466,30 +465,30 @@
     async def authorize_db_security_group_ingress(
         self,
         *,
         DBSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupId: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> AuthorizeDBSecurityGroupIngressResultTypeDef:
         """
         Enables ingress to a DBSecurityGroup using one of two forms of authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.authorize_db_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#authorize_db_security_group_ingress)
         """
 
     async def backtrack_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackTo: TimestampTypeDef,
         Force: bool = ...,
-        UseEarliestTimeOnPointInTimeUnavailable: bool = ...
+        UseEarliestTimeOnPointInTimeUnavailable: bool = ...,
     ) -> DBClusterBacktrackResponseTypeDef:
         """
         Backtracks a DB cluster to a specific time, without creating a new DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.backtrack_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#backtrack_db_cluster)
         """
@@ -522,15 +521,15 @@
 
     async def copy_db_cluster_parameter_group(
         self,
         *,
         SourceDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBClusterParameterGroupResultTypeDef:
         """
         Copies the specified DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_cluster_parameter_group)
         """
@@ -540,30 +539,30 @@
         *,
         SourceDBClusterSnapshotIdentifier: str,
         TargetDBClusterSnapshotIdentifier: str,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBClusterSnapshotResultTypeDef:
         """
         Copies a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_cluster_snapshot)
         """
 
     async def copy_db_parameter_group(
         self,
         *,
         SourceDBParameterGroupIdentifier: str,
         TargetDBParameterGroupIdentifier: str,
         TargetDBParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBParameterGroupResultTypeDef:
         """
         Copies the specified DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_parameter_group)
         """
@@ -576,30 +575,30 @@
         KmsKeyId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTags: bool = ...,
         PreSignedUrl: str = ...,
         OptionGroupName: str = ...,
         TargetCustomAvailabilityZone: str = ...,
         CopyOptionGroup: bool = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBSnapshotResultTypeDef:
         """
         Copies the specified DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_snapshot)
         """
 
     async def copy_option_group(
         self,
         *,
         SourceOptionGroupIdentifier: str,
         TargetOptionGroupIdentifier: str,
         TargetOptionGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyOptionGroupResultTypeDef:
         """
         Copies the specified option group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_option_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_option_group)
         """
@@ -610,15 +609,15 @@
         BlueGreenDeploymentName: str,
         Source: str,
         TargetEngineVersion: str = ...,
         TargetDBParameterGroupName: str = ...,
         TargetDBClusterParameterGroupName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TargetDBInstanceClass: str = ...,
-        UpgradeTargetStorageConfig: bool = ...
+        UpgradeTargetStorageConfig: bool = ...,
     ) -> CreateBlueGreenDeploymentResponseTypeDef:
         """
         Creates a blue/green deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_blue_green_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_blue_green_deployment)
         """
@@ -632,15 +631,15 @@
         DatabaseInstallationFilesS3Prefix: str = ...,
         ImageId: str = ...,
         KMSKeyId: str = ...,
         Description: str = ...,
         Manifest: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SourceCustomDbEngineVersionIdentifier: str = ...,
-        UseAwsProvidedLatestImage: bool = ...
+        UseAwsProvidedLatestImage: bool = ...,
     ) -> DBEngineVersionResponseTypeDef:
         """
         Creates a custom DB engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_custom_db_engine_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_custom_db_engine_version)
         """
@@ -695,15 +694,15 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         DBSystemId: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EnableLocalWriteForwarding: bool = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Aurora DB cluster or Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster)
         """
@@ -712,15 +711,15 @@
         self,
         *,
         DBClusterIdentifier: str,
         DBClusterEndpointIdentifier: str,
         EndpointType: str,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> DBClusterEndpointResponseTypeDef:
         """
         Creates a new custom endpoint and associates it with an Amazon Aurora DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster_endpoint)
@@ -728,29 +727,29 @@
 
     async def create_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterParameterGroupResultTypeDef:
         """
         Creates a new DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster_parameter_group)
         """
 
     async def create_db_cluster_snapshot(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         DBClusterIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterSnapshotResultTypeDef:
         """
         Creates a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster_snapshot)
         """
@@ -815,15 +814,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         CACertificateIdentifier: str = ...,
         DBSystemId: str = ...,
         DedicatedLogVolume: bool = ...,
-        MultiTenant: bool = ...
+        MultiTenant: bool = ...,
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_instance)
         """
@@ -871,15 +870,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         EnableCustomerOwnedIp: bool = ...,
         AllocatedStorage: int = ...,
         SourceDBClusterIdentifier: str = ...,
         DedicatedLogVolume: bool = ...,
         UpgradeStorageConfig: bool = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBInstanceReadReplicaResultTypeDef:
         """
         Creates a new DB instance that acts as a read replica for an existing source DB
         instance or Multi-AZ DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance_read_replica)
@@ -888,15 +887,15 @@
 
     async def create_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBParameterGroupResultTypeDef:
         """
         Creates a new DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_parameter_group)
         """
@@ -909,15 +908,15 @@
         Auth: Sequence[UserAuthConfigTypeDef],
         RoleArn: str,
         VpcSubnetIds: Sequence[str],
         VpcSecurityGroupIds: Sequence[str] = ...,
         RequireTLS: bool = ...,
         IdleClientTimeout: int = ...,
         DebugLogging: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBProxyResponseTypeDef:
         """
         Creates a new DB proxy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_proxy)
         """
@@ -926,58 +925,58 @@
         self,
         *,
         DBProxyName: str,
         DBProxyEndpointName: str,
         VpcSubnetIds: Sequence[str],
         VpcSecurityGroupIds: Sequence[str] = ...,
         TargetRole: DBProxyEndpointTargetRoleType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBProxyEndpointResponseTypeDef:
         """
         Creates a `DBProxyEndpoint`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_proxy_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_proxy_endpoint)
         """
 
     async def create_db_security_group(
         self,
         *,
         DBSecurityGroupName: str,
         DBSecurityGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSecurityGroupResultTypeDef:
         """
         Creates a new DB security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_security_group)
         """
 
     async def create_db_snapshot(
         self,
         *,
         DBSnapshotIdentifier: str,
         DBInstanceIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSnapshotResultTypeDef:
         """
         Creates a snapshot of a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_snapshot)
         """
 
     async def create_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         DBSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSubnetGroupResultTypeDef:
         """
         Creates a new DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_subnet_group)
         """
@@ -987,15 +986,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an RDS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_event_subscription)
         """
@@ -1005,15 +1004,15 @@
         *,
         GlobalClusterIdentifier: str = ...,
         SourceDBClusterIdentifier: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         DeletionProtection: bool = ...,
         DatabaseName: str = ...,
-        StorageEncrypted: bool = ...
+        StorageEncrypted: bool = ...,
     ) -> CreateGlobalClusterResultTypeDef:
         """
         Creates an Aurora global database spread across multiple Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_global_cluster)
@@ -1023,15 +1022,15 @@
         self,
         *,
         SourceArn: str,
         TargetArn: str,
         IntegrationName: str,
         KMSKeyId: str = ...,
         AdditionalEncryptionContext: Mapping[str, str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> IntegrationResponseTypeDef:
         """
         Creates a zero-ETL integration with Amazon Redshift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_integration)
         """
@@ -1039,15 +1038,15 @@
     async def create_option_group(
         self,
         *,
         OptionGroupName: str,
         EngineName: str,
         MajorEngineVersion: str,
         OptionGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOptionGroupResultTypeDef:
         """
         Creates a new option group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_option_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_option_group)
         """
@@ -1057,15 +1056,15 @@
         *,
         DBInstanceIdentifier: str,
         TenantDBName: str,
         MasterUsername: str,
         MasterUserPassword: str,
         CharacterSetName: str = ...,
         NcharCharacterSetName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTenantDatabaseResultTypeDef:
         """
         Creates a tenant database in a DB instance that uses the multi-tenant
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_tenant_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_tenant_database)
@@ -1093,15 +1092,15 @@
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
         FinalDBSnapshotIdentifier: str = ...,
-        DeleteAutomatedBackups: bool = ...
+        DeleteAutomatedBackups: bool = ...,
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_cluster)
         """
@@ -1150,15 +1149,15 @@
 
     async def delete_db_instance(
         self,
         *,
         DBInstanceIdentifier: str,
         SkipFinalSnapshot: bool = ...,
         FinalDBSnapshotIdentifier: str = ...,
-        DeleteAutomatedBackups: bool = ...
+        DeleteAutomatedBackups: bool = ...,
     ) -> DeleteDBInstanceResultTypeDef:
         """
         Deletes a previously provisioned DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_instance)
         """
@@ -1271,30 +1270,30 @@
 
     async def delete_tenant_database(
         self,
         *,
         DBInstanceIdentifier: str,
         TenantDBName: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteTenantDatabaseResultTypeDef:
         """
         Deletes a tenant database from your DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_tenant_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_tenant_database)
         """
 
     async def deregister_db_proxy_targets(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         DBInstanceIdentifiers: Sequence[str] = ...,
-        DBClusterIdentifiers: Sequence[str] = ...
+        DBClusterIdentifiers: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Remove the association between one or more `DBProxyTarget` data structures and
         a
         `DBProxyTargetGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.deregister_db_proxy_targets)
@@ -1311,30 +1310,30 @@
 
     async def describe_blue_green_deployments(
         self,
         *,
         BlueGreenDeploymentIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeBlueGreenDeploymentsResponseTypeDef:
         """
         Describes one or more blue/green deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_blue_green_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_blue_green_deployments)
         """
 
     async def describe_certificates(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CertificateMessageTypeDef:
         """
         Lists the set of certificate authority (CA) certificates provided by Amazon RDS
         for this Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_certificates)
@@ -1344,15 +1343,15 @@
     async def describe_db_cluster_automated_backups(
         self,
         *,
         DbClusterResourceId: str = ...,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterAutomatedBackupMessageTypeDef:
         """
         Displays backups for both current and deleted DB clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_automated_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_automated_backups)
         """
@@ -1360,15 +1359,15 @@
     async def describe_db_cluster_backtracks(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterBacktrackMessageTypeDef:
         """
         Returns information about backtracks for a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_backtracks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_backtracks)
         """
@@ -1376,30 +1375,30 @@
     async def describe_db_cluster_endpoints(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterEndpointMessageTypeDef:
         """
         Returns information about endpoints for an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_endpoints)
         """
 
     async def describe_db_cluster_parameter_groups(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBClusterParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_parameter_groups)
         """
@@ -1407,15 +1406,15 @@
     async def describe_db_cluster_parameters(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_parameters)
         """
@@ -1439,15 +1438,15 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...
+        DbClusterResourceId: str = ...,
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_snapshots)
         """
@@ -1455,15 +1454,15 @@
     async def describe_db_clusters(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        IncludeShared: bool = ...
+        IncludeShared: bool = ...,
     ) -> DBClusterMessageTypeDef:
         """
         Describes existing Amazon Aurora DB clusters and Multi-AZ DB clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_clusters)
         """
@@ -1476,15 +1475,15 @@
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        IncludeAll: bool = ...
+        IncludeAll: bool = ...,
     ) -> DBEngineVersionMessageTypeDef:
         """
         Describes the properties of specific versions of DB engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_engine_versions)
         """
@@ -1493,30 +1492,30 @@
         self,
         *,
         DbiResourceId: str = ...,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        DBInstanceAutomatedBackupsArn: str = ...
+        DBInstanceAutomatedBackupsArn: str = ...,
     ) -> DBInstanceAutomatedBackupMessageTypeDef:
         """
         Displays backups for both current and deleted instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_instance_automated_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_instance_automated_backups)
         """
 
     async def describe_db_instances(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBInstanceMessageTypeDef:
         """
         Describes provisioned RDS instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_instances)
         """
@@ -1526,30 +1525,30 @@
         *,
         DBInstanceIdentifier: str,
         FilenameContains: str = ...,
         FileLastWritten: int = ...,
         FileSize: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeDBLogFilesResponseTypeDef:
         """
         Returns a list of DB log files for the DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_log_files)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_log_files)
         """
 
     async def describe_db_parameter_groups(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_parameter_groups)
         """
@@ -1557,30 +1556,30 @@
     async def describe_db_parameters(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_parameters)
         """
 
     async def describe_db_proxies(
         self,
         *,
         DBProxyName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxiesResponseTypeDef:
         """
         Returns information about DB proxies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_proxies)
         """
@@ -1588,15 +1587,15 @@
     async def describe_db_proxy_endpoints(
         self,
         *,
         DBProxyName: str = ...,
         DBProxyEndpointName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxyEndpointsResponseTypeDef:
         """
         Returns information about DB proxy endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxy_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_proxy_endpoints)
         """
@@ -1604,15 +1603,15 @@
     async def describe_db_proxy_target_groups(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxyTargetGroupsResponseTypeDef:
         """
         Returns information about DB proxy target groups, represented by
         `DBProxyTargetGroup` data
         structures.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxy_target_groups)
@@ -1622,30 +1621,30 @@
     async def describe_db_proxy_targets(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxyTargetsResponseTypeDef:
         """
         Returns information about `DBProxyTarget` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxy_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_proxy_targets)
         """
 
     async def describe_db_security_groups(
         self,
         *,
         DBSecurityGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSecurityGroupMessageTypeDef:
         """
         Returns a list of `DBSecurityGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_security_groups)
         """
@@ -1666,15 +1665,15 @@
         *,
         DBInstanceIdentifier: str = ...,
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        DbiResourceId: str = ...
+        DbiResourceId: str = ...,
     ) -> DBSnapshotTenantDatabasesMessageTypeDef:
         """
         Describes the tenant databases that exist in a DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_snapshot_tenant_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_snapshot_tenant_databases)
         """
@@ -1686,45 +1685,45 @@
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbiResourceId: str = ...
+        DbiResourceId: str = ...,
     ) -> DBSnapshotMessageTypeDef:
         """
         Returns information about DB snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_snapshots)
         """
 
     async def describe_db_subnet_groups(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSubnetGroupMessageTypeDef:
         """
         Returns a list of DBSubnetGroup descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_subnet_groups)
         """
 
     async def describe_engine_default_cluster_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultClusterParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the cluster
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_engine_default_cluster_parameters)
@@ -1733,15 +1732,15 @@
 
     async def describe_engine_default_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the specified
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_engine_default_parameters)
@@ -1762,15 +1761,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists all the subscription descriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_event_subscriptions)
         """
@@ -1782,15 +1781,15 @@
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to DB instances, DB clusters, DB parameter groups, DB
         security groups, DB snapshots, DB cluster snapshots, and RDS Proxies for the
         past 14
         days.
 
@@ -1802,45 +1801,45 @@
         self,
         *,
         ExportTaskIdentifier: str = ...,
         SourceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        SourceType: ExportSourceTypeType = ...
+        SourceType: ExportSourceTypeType = ...,
     ) -> ExportTasksMessageTypeDef:
         """
         Returns information about a snapshot or cluster export to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_export_tasks)
         """
 
     async def describe_global_clusters(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GlobalClustersMessageTypeDef:
         """
         Returns information about Aurora global database clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_global_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_global_clusters)
         """
 
     async def describe_integrations(
         self,
         *,
         IntegrationIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeIntegrationsResponseTypeDef:
         """
         Describe one or more zero-ETL integrations with Amazon Redshift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_integrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_integrations)
         """
@@ -1848,15 +1847,15 @@
     async def describe_option_group_options(
         self,
         *,
         EngineName: str,
         MajorEngineVersion: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OptionGroupOptionsMessageTypeDef:
         """
         Describes all available options for the specified engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_option_group_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_option_group_options)
         """
@@ -1865,15 +1864,15 @@
         self,
         *,
         OptionGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
         EngineName: str = ...,
-        MajorEngineVersion: str = ...
+        MajorEngineVersion: str = ...,
     ) -> OptionGroupsTypeDef:
         """
         Describes the available option groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_option_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_option_groups)
         """
@@ -1885,30 +1884,30 @@
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         AvailabilityZoneGroup: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableDBInstanceOptionsMessageTypeDef:
         """
         Describes the orderable DB instance options for a specified DB engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_orderable_db_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_orderable_db_instance_options)
         """
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PendingMaintenanceActionsMessageTypeDef:
         """
         Returns a list of resources (for example, DB instances) that have at least one
         pending maintenance
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_pending_maintenance_actions)
@@ -1924,15 +1923,15 @@
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         LeaseId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedDBInstanceMessageTypeDef:
         """
         Returns information about reserved DB instances for this account, or about a
         specified reserved DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_reserved_db_instances)
@@ -1946,30 +1945,30 @@
         DBInstanceClass: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedDBInstancesOfferingMessageTypeDef:
         """
         Lists available reserved DB instance offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_reserved_db_instances_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_reserved_db_instances_offerings)
         """
 
     async def describe_source_regions(
         self,
         *,
         RegionName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> SourceRegionMessageTypeDef:
         """
         Returns a list of the source Amazon Web Services Regions where the current
         Amazon Web Services Region can create a read replica, copy a DB snapshot from,
         or replicate automated backups
         from.
 
@@ -1980,15 +1979,15 @@
     async def describe_tenant_databases(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> TenantDatabasesMessageTypeDef:
         """
         Describes the tenant databases in a DB instance that uses the multi-tenant
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_tenant_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_tenant_databases)
@@ -2008,15 +2007,15 @@
 
     async def download_db_log_file_portion(
         self,
         *,
         DBInstanceIdentifier: str,
         LogFileName: str,
         Marker: str = ...,
-        NumberOfLines: int = ...
+        NumberOfLines: int = ...,
     ) -> DownloadDBLogFilePortionDetailsTypeDef:
         """
         Downloads all or a portion of the specified log file, up to 1 MB in size.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.download_db_log_file_portion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#download_db_log_file_portion)
         """
@@ -2033,15 +2032,15 @@
 
     async def failover_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str,
         TargetDbClusterIdentifier: str,
         AllowDataLoss: bool = ...,
-        Switchover: bool = ...
+        Switchover: bool = ...,
     ) -> FailoverGlobalClusterResultTypeDef:
         """
         Promotes the specified secondary DB cluster to be the primary DB cluster in the
         global database cluster to fail over or switch over a global
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.failover_global_cluster)
@@ -2108,30 +2107,30 @@
 
     async def modify_current_db_cluster_capacity(
         self,
         *,
         DBClusterIdentifier: str,
         Capacity: int = ...,
         SecondsBeforeTimeout: int = ...,
-        TimeoutAction: str = ...
+        TimeoutAction: str = ...,
     ) -> DBClusterCapacityInfoTypeDef:
         """
         Set the capacity of an Aurora Serverless v1 DB cluster to a specific value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_current_db_cluster_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_current_db_cluster_capacity)
         """
 
     async def modify_custom_db_engine_version(
         self,
         *,
         Engine: str,
         EngineVersion: str,
         Description: str = ...,
-        Status: CustomEngineVersionStatusType = ...
+        Status: CustomEngineVersionStatusType = ...,
     ) -> DBEngineVersionResponseTypeDef:
         """
         Modifies the status of a custom engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_custom_db_engine_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_custom_db_engine_version)
         """
@@ -2177,30 +2176,30 @@
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EngineMode: str = ...,
         AllowEngineModeChange: bool = ...,
         EnableLocalWriteForwarding: bool = ...,
-        AwsBackupRecoveryPointArn: str = ...
+        AwsBackupRecoveryPointArn: str = ...,
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies the settings of an Amazon Aurora DB cluster or a Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster)
         """
 
     async def modify_db_cluster_endpoint(
         self,
         *,
         DBClusterEndpointIdentifier: str,
         EndpointType: str = ...,
         StaticMembers: Sequence[str] = ...,
-        ExcludedMembers: Sequence[str] = ...
+        ExcludedMembers: Sequence[str] = ...,
     ) -> DBClusterEndpointResponseTypeDef:
         """
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster_endpoint)
         """
@@ -2217,15 +2216,15 @@
 
     async def modify_db_cluster_snapshot_attribute(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBClusterSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual DB cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_snapshot_attribute)
@@ -2290,15 +2289,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         Engine: str = ...,
         DedicatedLogVolume: bool = ...,
-        MultiTenant: bool = ...
+        MultiTenant: bool = ...,
     ) -> ModifyDBInstanceResultTypeDef:
         """
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_instance)
         """
@@ -2319,44 +2318,44 @@
         DBProxyName: str,
         NewDBProxyName: str = ...,
         Auth: Sequence[UserAuthConfigTypeDef] = ...,
         RequireTLS: bool = ...,
         IdleClientTimeout: int = ...,
         DebugLogging: bool = ...,
         RoleArn: str = ...,
-        SecurityGroups: Sequence[str] = ...
+        SecurityGroups: Sequence[str] = ...,
     ) -> ModifyDBProxyResponseTypeDef:
         """
         Changes the settings for an existing DB proxy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_proxy)
         """
 
     async def modify_db_proxy_endpoint(
         self,
         *,
         DBProxyEndpointName: str,
         NewDBProxyEndpointName: str = ...,
-        VpcSecurityGroupIds: Sequence[str] = ...
+        VpcSecurityGroupIds: Sequence[str] = ...,
     ) -> ModifyDBProxyEndpointResponseTypeDef:
         """
         Changes the settings for an existing DB proxy endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_proxy_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_proxy_endpoint)
         """
 
     async def modify_db_proxy_target_group(
         self,
         *,
         TargetGroupName: str,
         DBProxyName: str,
         ConnectionPoolConfig: ConnectionPoolConfigurationTypeDef = ...,
-        NewName: str = ...
+        NewName: str = ...,
     ) -> ModifyDBProxyTargetGroupResponseTypeDef:
         """
         Modifies the properties of a `DBProxyTargetGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_proxy_target_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_proxy_target_group)
         """
@@ -2373,15 +2372,15 @@
 
     async def modify_db_snapshot_attribute(
         self,
         *,
         DBSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual DB
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_snapshot_attribute)
@@ -2389,15 +2388,15 @@
         """
 
     async def modify_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         SubnetIds: Sequence[str],
-        DBSubnetGroupDescription: str = ...
+        DBSubnetGroupDescription: str = ...,
     ) -> ModifyDBSubnetGroupResultTypeDef:
         """
         Modifies an existing DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_subnet_group)
         """
@@ -2405,15 +2404,15 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing RDS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_event_subscription)
         """
@@ -2421,59 +2420,59 @@
     async def modify_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
-        AllowMajorVersionUpgrade: bool = ...
+        AllowMajorVersionUpgrade: bool = ...,
     ) -> ModifyGlobalClusterResultTypeDef:
         """
         Modifies a setting for an Amazon Aurora global database cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_global_cluster)
         """
 
     async def modify_option_group(
         self,
         *,
         OptionGroupName: str,
         OptionsToInclude: Sequence[OptionConfigurationTypeDef] = ...,
         OptionsToRemove: Sequence[str] = ...,
-        ApplyImmediately: bool = ...
+        ApplyImmediately: bool = ...,
     ) -> ModifyOptionGroupResultTypeDef:
         """
         Modifies an existing option group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_option_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_option_group)
         """
 
     async def modify_tenant_database(
         self,
         *,
         DBInstanceIdentifier: str,
         TenantDBName: str,
         MasterUserPassword: str = ...,
-        NewTenantDBName: str = ...
+        NewTenantDBName: str = ...,
     ) -> ModifyTenantDatabaseResultTypeDef:
         """
         Modifies an existing tenant database in a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_tenant_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_tenant_database)
         """
 
     async def promote_read_replica(
         self,
         *,
         DBInstanceIdentifier: str,
         BackupRetentionPeriod: int = ...,
-        PreferredBackupWindow: str = ...
+        PreferredBackupWindow: str = ...,
     ) -> PromoteReadReplicaResultTypeDef:
         """
         Promotes a read replica DB instance to a standalone DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.promote_read_replica)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#promote_read_replica)
         """
@@ -2490,15 +2489,15 @@
 
     async def purchase_reserved_db_instances_offering(
         self,
         *,
         ReservedDBInstancesOfferingId: str,
         ReservedDBInstanceId: str = ...,
         DBInstanceCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PurchaseReservedDBInstancesOfferingResultTypeDef:
         """
         Purchases a reserved DB instance offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.purchase_reserved_db_instances_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#purchase_reserved_db_instances_offering)
         """
@@ -2523,15 +2522,15 @@
 
     async def register_db_proxy_targets(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         DBInstanceIdentifiers: Sequence[str] = ...,
-        DBClusterIdentifiers: Sequence[str] = ...
+        DBClusterIdentifiers: Sequence[str] = ...,
     ) -> RegisterDBProxyTargetsResponseTypeDef:
         """
         Associate one or more `DBProxyTarget` data structures with a
         `DBProxyTargetGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.register_db_proxy_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#register_db_proxy_targets)
@@ -2593,29 +2592,29 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_cluster_parameter_group)
         """
 
     async def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_parameter_group)
@@ -2655,15 +2654,15 @@
         CopyTagsToSnapshot: bool = ...,
         Domain: str = ...,
         DomainIAMRoleName: str = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterFromS3ResultTypeDef:
         """
         Creates an Amazon Aurora DB cluster from MySQL data stored in an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_from_s3)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_from_s3)
@@ -2696,15 +2695,15 @@
         DomainIAMRoleName: str = ...,
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         Iops: int = ...,
         PubliclyAccessible: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
-        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...
+        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...,
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new DB cluster from a DB snapshot or DB cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_from_snapshot)
         """
@@ -2736,15 +2735,15 @@
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         PubliclyAccessible: bool = ...,
         Iops: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         SourceDbClusterResourceId: str = ...,
-        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...
+        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...,
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_to_point_in_time)
         """
@@ -2787,15 +2786,15 @@
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         DBClusterSnapshotIdentifier: str = ...,
         AllocatedStorage: int = ...,
-        DedicatedLogVolume: bool = ...
+        DedicatedLogVolume: bool = ...,
     ) -> RestoreDBInstanceFromDBSnapshotResultTypeDef:
         """
         Creates a new DB instance from a DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_db_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_instance_from_db_snapshot)
         """
@@ -2847,15 +2846,15 @@
         UseDefaultProcessorFeatures: bool = ...,
         DeletionProtection: bool = ...,
         MaxAllocatedStorage: int = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        DedicatedLogVolume: bool = ...
+        DedicatedLogVolume: bool = ...,
     ) -> RestoreDBInstanceFromS3ResultTypeDef:
         """
         Amazon Relational Database Service (Amazon RDS) supports importing MySQL
         databases by using backup
         files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_s3)
@@ -2904,15 +2903,15 @@
         SourceDBInstanceAutomatedBackupsArn: str = ...,
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         AllocatedStorage: int = ...,
-        DedicatedLogVolume: bool = ...
+        DedicatedLogVolume: bool = ...,
     ) -> RestoreDBInstanceToPointInTimeResultTypeDef:
         """
         Restores a DB instance to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_instance_to_point_in_time)
         """
@@ -2920,15 +2919,15 @@
     async def revoke_db_security_group_ingress(
         self,
         *,
         DBSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupId: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> RevokeDBSecurityGroupIngressResultTypeDef:
         """
         Revokes ingress from a DBSecurityGroup for previously authorized IP ranges or
         EC2 or VPC security
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.revoke_db_security_group_ingress)
@@ -2938,15 +2937,15 @@
     async def start_activity_stream(
         self,
         *,
         ResourceArn: str,
         Mode: ActivityStreamModeType,
         KmsKeyId: str,
         ApplyImmediately: bool = ...,
-        EngineNativeAuditFieldsIncluded: bool = ...
+        EngineNativeAuditFieldsIncluded: bool = ...,
     ) -> StartActivityStreamResponseTypeDef:
         """
         Starts a database activity stream to monitor activity on the database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_activity_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#start_activity_stream)
         """
@@ -2974,15 +2973,15 @@
     async def start_db_instance_automated_backups_replication(
         self,
         *,
         SourceDBInstanceArn: str,
         BackupRetentionPeriod: int = ...,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> StartDBInstanceAutomatedBackupsReplicationResultTypeDef:
         """
         Enables replication of automated backups to a different Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_db_instance_automated_backups_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#start_db_instance_automated_backups_replication)
@@ -2993,15 +2992,15 @@
         *,
         ExportTaskIdentifier: str,
         SourceArn: str,
         S3BucketName: str,
         IamRoleArn: str,
         KmsKeyId: str,
         S3Prefix: str = ...,
-        ExportOnly: Sequence[str] = ...
+        ExportOnly: Sequence[str] = ...,
     ) -> ExportTaskResponseTypeDef:
         """
         Starts an export of DB snapshot or DB cluster data to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#start_export_task)
         """
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/client.pyi` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -462,30 +462,30 @@
     async def authorize_db_security_group_ingress(
         self,
         *,
         DBSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupId: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> AuthorizeDBSecurityGroupIngressResultTypeDef:
         """
         Enables ingress to a DBSecurityGroup using one of two forms of authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.authorize_db_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#authorize_db_security_group_ingress)
         """
 
     async def backtrack_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackTo: TimestampTypeDef,
         Force: bool = ...,
-        UseEarliestTimeOnPointInTimeUnavailable: bool = ...
+        UseEarliestTimeOnPointInTimeUnavailable: bool = ...,
     ) -> DBClusterBacktrackResponseTypeDef:
         """
         Backtracks a DB cluster to a specific time, without creating a new DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.backtrack_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#backtrack_db_cluster)
         """
@@ -518,15 +518,15 @@
 
     async def copy_db_cluster_parameter_group(
         self,
         *,
         SourceDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBClusterParameterGroupResultTypeDef:
         """
         Copies the specified DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_cluster_parameter_group)
         """
@@ -536,30 +536,30 @@
         *,
         SourceDBClusterSnapshotIdentifier: str,
         TargetDBClusterSnapshotIdentifier: str,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBClusterSnapshotResultTypeDef:
         """
         Copies a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_cluster_snapshot)
         """
 
     async def copy_db_parameter_group(
         self,
         *,
         SourceDBParameterGroupIdentifier: str,
         TargetDBParameterGroupIdentifier: str,
         TargetDBParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBParameterGroupResultTypeDef:
         """
         Copies the specified DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_parameter_group)
         """
@@ -572,30 +572,30 @@
         KmsKeyId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTags: bool = ...,
         PreSignedUrl: str = ...,
         OptionGroupName: str = ...,
         TargetCustomAvailabilityZone: str = ...,
         CopyOptionGroup: bool = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBSnapshotResultTypeDef:
         """
         Copies the specified DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_db_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_db_snapshot)
         """
 
     async def copy_option_group(
         self,
         *,
         SourceOptionGroupIdentifier: str,
         TargetOptionGroupIdentifier: str,
         TargetOptionGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyOptionGroupResultTypeDef:
         """
         Copies the specified option group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.copy_option_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#copy_option_group)
         """
@@ -606,15 +606,15 @@
         BlueGreenDeploymentName: str,
         Source: str,
         TargetEngineVersion: str = ...,
         TargetDBParameterGroupName: str = ...,
         TargetDBClusterParameterGroupName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TargetDBInstanceClass: str = ...,
-        UpgradeTargetStorageConfig: bool = ...
+        UpgradeTargetStorageConfig: bool = ...,
     ) -> CreateBlueGreenDeploymentResponseTypeDef:
         """
         Creates a blue/green deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_blue_green_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_blue_green_deployment)
         """
@@ -628,15 +628,15 @@
         DatabaseInstallationFilesS3Prefix: str = ...,
         ImageId: str = ...,
         KMSKeyId: str = ...,
         Description: str = ...,
         Manifest: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SourceCustomDbEngineVersionIdentifier: str = ...,
-        UseAwsProvidedLatestImage: bool = ...
+        UseAwsProvidedLatestImage: bool = ...,
     ) -> DBEngineVersionResponseTypeDef:
         """
         Creates a custom DB engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_custom_db_engine_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_custom_db_engine_version)
         """
@@ -691,15 +691,15 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         DBSystemId: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EnableLocalWriteForwarding: bool = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Aurora DB cluster or Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster)
         """
@@ -708,15 +708,15 @@
         self,
         *,
         DBClusterIdentifier: str,
         DBClusterEndpointIdentifier: str,
         EndpointType: str,
         StaticMembers: Sequence[str] = ...,
         ExcludedMembers: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> DBClusterEndpointResponseTypeDef:
         """
         Creates a new custom endpoint and associates it with an Amazon Aurora DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster_endpoint)
@@ -724,29 +724,29 @@
 
     async def create_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterParameterGroupResultTypeDef:
         """
         Creates a new DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster_parameter_group)
         """
 
     async def create_db_cluster_snapshot(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         DBClusterIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterSnapshotResultTypeDef:
         """
         Creates a snapshot of a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster_snapshot)
         """
@@ -811,15 +811,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         CACertificateIdentifier: str = ...,
         DBSystemId: str = ...,
         DedicatedLogVolume: bool = ...,
-        MultiTenant: bool = ...
+        MultiTenant: bool = ...,
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_instance)
         """
@@ -867,15 +867,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         EnableCustomerOwnedIp: bool = ...,
         AllocatedStorage: int = ...,
         SourceDBClusterIdentifier: str = ...,
         DedicatedLogVolume: bool = ...,
         UpgradeStorageConfig: bool = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBInstanceReadReplicaResultTypeDef:
         """
         Creates a new DB instance that acts as a read replica for an existing source DB
         instance or Multi-AZ DB
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance_read_replica)
@@ -884,15 +884,15 @@
 
     async def create_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBParameterGroupResultTypeDef:
         """
         Creates a new DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_parameter_group)
         """
@@ -905,15 +905,15 @@
         Auth: Sequence[UserAuthConfigTypeDef],
         RoleArn: str,
         VpcSubnetIds: Sequence[str],
         VpcSecurityGroupIds: Sequence[str] = ...,
         RequireTLS: bool = ...,
         IdleClientTimeout: int = ...,
         DebugLogging: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBProxyResponseTypeDef:
         """
         Creates a new DB proxy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_proxy)
         """
@@ -922,58 +922,58 @@
         self,
         *,
         DBProxyName: str,
         DBProxyEndpointName: str,
         VpcSubnetIds: Sequence[str],
         VpcSecurityGroupIds: Sequence[str] = ...,
         TargetRole: DBProxyEndpointTargetRoleType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBProxyEndpointResponseTypeDef:
         """
         Creates a `DBProxyEndpoint`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_proxy_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_proxy_endpoint)
         """
 
     async def create_db_security_group(
         self,
         *,
         DBSecurityGroupName: str,
         DBSecurityGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSecurityGroupResultTypeDef:
         """
         Creates a new DB security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_security_group)
         """
 
     async def create_db_snapshot(
         self,
         *,
         DBSnapshotIdentifier: str,
         DBInstanceIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSnapshotResultTypeDef:
         """
         Creates a snapshot of a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_snapshot)
         """
 
     async def create_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         DBSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSubnetGroupResultTypeDef:
         """
         Creates a new DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_subnet_group)
         """
@@ -983,15 +983,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an RDS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_event_subscription)
         """
@@ -1001,15 +1001,15 @@
         *,
         GlobalClusterIdentifier: str = ...,
         SourceDBClusterIdentifier: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         DeletionProtection: bool = ...,
         DatabaseName: str = ...,
-        StorageEncrypted: bool = ...
+        StorageEncrypted: bool = ...,
     ) -> CreateGlobalClusterResultTypeDef:
         """
         Creates an Aurora global database spread across multiple Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_global_cluster)
@@ -1019,15 +1019,15 @@
         self,
         *,
         SourceArn: str,
         TargetArn: str,
         IntegrationName: str,
         KMSKeyId: str = ...,
         AdditionalEncryptionContext: Mapping[str, str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> IntegrationResponseTypeDef:
         """
         Creates a zero-ETL integration with Amazon Redshift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_integration)
         """
@@ -1035,15 +1035,15 @@
     async def create_option_group(
         self,
         *,
         OptionGroupName: str,
         EngineName: str,
         MajorEngineVersion: str,
         OptionGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOptionGroupResultTypeDef:
         """
         Creates a new option group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_option_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_option_group)
         """
@@ -1053,15 +1053,15 @@
         *,
         DBInstanceIdentifier: str,
         TenantDBName: str,
         MasterUsername: str,
         MasterUserPassword: str,
         CharacterSetName: str = ...,
         NcharCharacterSetName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTenantDatabaseResultTypeDef:
         """
         Creates a tenant database in a DB instance that uses the multi-tenant
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_tenant_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_tenant_database)
@@ -1089,15 +1089,15 @@
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
         FinalDBSnapshotIdentifier: str = ...,
-        DeleteAutomatedBackups: bool = ...
+        DeleteAutomatedBackups: bool = ...,
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_cluster)
         """
@@ -1146,15 +1146,15 @@
 
     async def delete_db_instance(
         self,
         *,
         DBInstanceIdentifier: str,
         SkipFinalSnapshot: bool = ...,
         FinalDBSnapshotIdentifier: str = ...,
-        DeleteAutomatedBackups: bool = ...
+        DeleteAutomatedBackups: bool = ...,
     ) -> DeleteDBInstanceResultTypeDef:
         """
         Deletes a previously provisioned DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_instance)
         """
@@ -1267,30 +1267,30 @@
 
     async def delete_tenant_database(
         self,
         *,
         DBInstanceIdentifier: str,
         TenantDBName: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteTenantDatabaseResultTypeDef:
         """
         Deletes a tenant database from your DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_tenant_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_tenant_database)
         """
 
     async def deregister_db_proxy_targets(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         DBInstanceIdentifiers: Sequence[str] = ...,
-        DBClusterIdentifiers: Sequence[str] = ...
+        DBClusterIdentifiers: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Remove the association between one or more `DBProxyTarget` data structures and
         a
         `DBProxyTargetGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.deregister_db_proxy_targets)
@@ -1307,30 +1307,30 @@
 
     async def describe_blue_green_deployments(
         self,
         *,
         BlueGreenDeploymentIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeBlueGreenDeploymentsResponseTypeDef:
         """
         Describes one or more blue/green deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_blue_green_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_blue_green_deployments)
         """
 
     async def describe_certificates(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CertificateMessageTypeDef:
         """
         Lists the set of certificate authority (CA) certificates provided by Amazon RDS
         for this Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_certificates)
@@ -1340,15 +1340,15 @@
     async def describe_db_cluster_automated_backups(
         self,
         *,
         DbClusterResourceId: str = ...,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterAutomatedBackupMessageTypeDef:
         """
         Displays backups for both current and deleted DB clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_automated_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_automated_backups)
         """
@@ -1356,15 +1356,15 @@
     async def describe_db_cluster_backtracks(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterBacktrackMessageTypeDef:
         """
         Returns information about backtracks for a DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_backtracks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_backtracks)
         """
@@ -1372,30 +1372,30 @@
     async def describe_db_cluster_endpoints(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterEndpointMessageTypeDef:
         """
         Returns information about endpoints for an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_endpoints)
         """
 
     async def describe_db_cluster_parameter_groups(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBClusterParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_parameter_groups)
         """
@@ -1403,15 +1403,15 @@
     async def describe_db_cluster_parameters(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_parameters)
         """
@@ -1435,15 +1435,15 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbClusterResourceId: str = ...
+        DbClusterResourceId: str = ...,
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_snapshots)
         """
@@ -1451,15 +1451,15 @@
     async def describe_db_clusters(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        IncludeShared: bool = ...
+        IncludeShared: bool = ...,
     ) -> DBClusterMessageTypeDef:
         """
         Describes existing Amazon Aurora DB clusters and Multi-AZ DB clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_clusters)
         """
@@ -1472,15 +1472,15 @@
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        IncludeAll: bool = ...
+        IncludeAll: bool = ...,
     ) -> DBEngineVersionMessageTypeDef:
         """
         Describes the properties of specific versions of DB engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_engine_versions)
         """
@@ -1489,30 +1489,30 @@
         self,
         *,
         DbiResourceId: str = ...,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        DBInstanceAutomatedBackupsArn: str = ...
+        DBInstanceAutomatedBackupsArn: str = ...,
     ) -> DBInstanceAutomatedBackupMessageTypeDef:
         """
         Displays backups for both current and deleted instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_instance_automated_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_instance_automated_backups)
         """
 
     async def describe_db_instances(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBInstanceMessageTypeDef:
         """
         Describes provisioned RDS instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_instances)
         """
@@ -1522,30 +1522,30 @@
         *,
         DBInstanceIdentifier: str,
         FilenameContains: str = ...,
         FileLastWritten: int = ...,
         FileSize: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeDBLogFilesResponseTypeDef:
         """
         Returns a list of DB log files for the DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_log_files)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_log_files)
         """
 
     async def describe_db_parameter_groups(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_parameter_groups)
         """
@@ -1553,30 +1553,30 @@
     async def describe_db_parameters(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_parameters)
         """
 
     async def describe_db_proxies(
         self,
         *,
         DBProxyName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxiesResponseTypeDef:
         """
         Returns information about DB proxies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_proxies)
         """
@@ -1584,15 +1584,15 @@
     async def describe_db_proxy_endpoints(
         self,
         *,
         DBProxyName: str = ...,
         DBProxyEndpointName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxyEndpointsResponseTypeDef:
         """
         Returns information about DB proxy endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxy_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_proxy_endpoints)
         """
@@ -1600,15 +1600,15 @@
     async def describe_db_proxy_target_groups(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxyTargetGroupsResponseTypeDef:
         """
         Returns information about DB proxy target groups, represented by
         `DBProxyTargetGroup` data
         structures.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxy_target_groups)
@@ -1618,30 +1618,30 @@
     async def describe_db_proxy_targets(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeDBProxyTargetsResponseTypeDef:
         """
         Returns information about `DBProxyTarget` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_proxy_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_proxy_targets)
         """
 
     async def describe_db_security_groups(
         self,
         *,
         DBSecurityGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSecurityGroupMessageTypeDef:
         """
         Returns a list of `DBSecurityGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_security_groups)
         """
@@ -1662,15 +1662,15 @@
         *,
         DBInstanceIdentifier: str = ...,
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        DbiResourceId: str = ...
+        DbiResourceId: str = ...,
     ) -> DBSnapshotTenantDatabasesMessageTypeDef:
         """
         Describes the tenant databases that exist in a DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_snapshot_tenant_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_snapshot_tenant_databases)
         """
@@ -1682,45 +1682,45 @@
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        DbiResourceId: str = ...
+        DbiResourceId: str = ...,
     ) -> DBSnapshotMessageTypeDef:
         """
         Returns information about DB snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_snapshots)
         """
 
     async def describe_db_subnet_groups(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSubnetGroupMessageTypeDef:
         """
         Returns a list of DBSubnetGroup descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_subnet_groups)
         """
 
     async def describe_engine_default_cluster_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultClusterParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the cluster
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_engine_default_cluster_parameters)
@@ -1729,15 +1729,15 @@
 
     async def describe_engine_default_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the specified
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_engine_default_parameters)
@@ -1758,15 +1758,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists all the subscription descriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_event_subscriptions)
         """
@@ -1778,15 +1778,15 @@
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to DB instances, DB clusters, DB parameter groups, DB
         security groups, DB snapshots, DB cluster snapshots, and RDS Proxies for the
         past 14
         days.
 
@@ -1798,45 +1798,45 @@
         self,
         *,
         ExportTaskIdentifier: str = ...,
         SourceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        SourceType: ExportSourceTypeType = ...
+        SourceType: ExportSourceTypeType = ...,
     ) -> ExportTasksMessageTypeDef:
         """
         Returns information about a snapshot or cluster export to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_export_tasks)
         """
 
     async def describe_global_clusters(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GlobalClustersMessageTypeDef:
         """
         Returns information about Aurora global database clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_global_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_global_clusters)
         """
 
     async def describe_integrations(
         self,
         *,
         IntegrationIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeIntegrationsResponseTypeDef:
         """
         Describe one or more zero-ETL integrations with Amazon Redshift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_integrations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_integrations)
         """
@@ -1844,15 +1844,15 @@
     async def describe_option_group_options(
         self,
         *,
         EngineName: str,
         MajorEngineVersion: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OptionGroupOptionsMessageTypeDef:
         """
         Describes all available options for the specified engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_option_group_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_option_group_options)
         """
@@ -1861,15 +1861,15 @@
         self,
         *,
         OptionGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
         EngineName: str = ...,
-        MajorEngineVersion: str = ...
+        MajorEngineVersion: str = ...,
     ) -> OptionGroupsTypeDef:
         """
         Describes the available option groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_option_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_option_groups)
         """
@@ -1881,30 +1881,30 @@
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         AvailabilityZoneGroup: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableDBInstanceOptionsMessageTypeDef:
         """
         Describes the orderable DB instance options for a specified DB engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_orderable_db_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_orderable_db_instance_options)
         """
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PendingMaintenanceActionsMessageTypeDef:
         """
         Returns a list of resources (for example, DB instances) that have at least one
         pending maintenance
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_pending_maintenance_actions)
@@ -1920,15 +1920,15 @@
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         LeaseId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedDBInstanceMessageTypeDef:
         """
         Returns information about reserved DB instances for this account, or about a
         specified reserved DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_reserved_db_instances)
@@ -1942,30 +1942,30 @@
         DBInstanceClass: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> ReservedDBInstancesOfferingMessageTypeDef:
         """
         Lists available reserved DB instance offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_reserved_db_instances_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_reserved_db_instances_offerings)
         """
 
     async def describe_source_regions(
         self,
         *,
         RegionName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> SourceRegionMessageTypeDef:
         """
         Returns a list of the source Amazon Web Services Regions where the current
         Amazon Web Services Region can create a read replica, copy a DB snapshot from,
         or replicate automated backups
         from.
 
@@ -1976,15 +1976,15 @@
     async def describe_tenant_databases(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> TenantDatabasesMessageTypeDef:
         """
         Describes the tenant databases in a DB instance that uses the multi-tenant
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_tenant_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_tenant_databases)
@@ -2004,15 +2004,15 @@
 
     async def download_db_log_file_portion(
         self,
         *,
         DBInstanceIdentifier: str,
         LogFileName: str,
         Marker: str = ...,
-        NumberOfLines: int = ...
+        NumberOfLines: int = ...,
     ) -> DownloadDBLogFilePortionDetailsTypeDef:
         """
         Downloads all or a portion of the specified log file, up to 1 MB in size.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.download_db_log_file_portion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#download_db_log_file_portion)
         """
@@ -2029,15 +2029,15 @@
 
     async def failover_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str,
         TargetDbClusterIdentifier: str,
         AllowDataLoss: bool = ...,
-        Switchover: bool = ...
+        Switchover: bool = ...,
     ) -> FailoverGlobalClusterResultTypeDef:
         """
         Promotes the specified secondary DB cluster to be the primary DB cluster in the
         global database cluster to fail over or switch over a global
         database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.failover_global_cluster)
@@ -2104,30 +2104,30 @@
 
     async def modify_current_db_cluster_capacity(
         self,
         *,
         DBClusterIdentifier: str,
         Capacity: int = ...,
         SecondsBeforeTimeout: int = ...,
-        TimeoutAction: str = ...
+        TimeoutAction: str = ...,
     ) -> DBClusterCapacityInfoTypeDef:
         """
         Set the capacity of an Aurora Serverless v1 DB cluster to a specific value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_current_db_cluster_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_current_db_cluster_capacity)
         """
 
     async def modify_custom_db_engine_version(
         self,
         *,
         Engine: str,
         EngineVersion: str,
         Description: str = ...,
-        Status: CustomEngineVersionStatusType = ...
+        Status: CustomEngineVersionStatusType = ...,
     ) -> DBEngineVersionResponseTypeDef:
         """
         Modifies the status of a custom engine version (CEV).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_custom_db_engine_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_custom_db_engine_version)
         """
@@ -2173,30 +2173,30 @@
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EngineMode: str = ...,
         AllowEngineModeChange: bool = ...,
         EnableLocalWriteForwarding: bool = ...,
-        AwsBackupRecoveryPointArn: str = ...
+        AwsBackupRecoveryPointArn: str = ...,
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies the settings of an Amazon Aurora DB cluster or a Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster)
         """
 
     async def modify_db_cluster_endpoint(
         self,
         *,
         DBClusterEndpointIdentifier: str,
         EndpointType: str = ...,
         StaticMembers: Sequence[str] = ...,
-        ExcludedMembers: Sequence[str] = ...
+        ExcludedMembers: Sequence[str] = ...,
     ) -> DBClusterEndpointResponseTypeDef:
         """
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster_endpoint)
         """
@@ -2213,15 +2213,15 @@
 
     async def modify_db_cluster_snapshot_attribute(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBClusterSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual DB cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_snapshot_attribute)
@@ -2286,15 +2286,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         Engine: str = ...,
         DedicatedLogVolume: bool = ...,
-        MultiTenant: bool = ...
+        MultiTenant: bool = ...,
     ) -> ModifyDBInstanceResultTypeDef:
         """
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_instance)
         """
@@ -2315,44 +2315,44 @@
         DBProxyName: str,
         NewDBProxyName: str = ...,
         Auth: Sequence[UserAuthConfigTypeDef] = ...,
         RequireTLS: bool = ...,
         IdleClientTimeout: int = ...,
         DebugLogging: bool = ...,
         RoleArn: str = ...,
-        SecurityGroups: Sequence[str] = ...
+        SecurityGroups: Sequence[str] = ...,
     ) -> ModifyDBProxyResponseTypeDef:
         """
         Changes the settings for an existing DB proxy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_proxy)
         """
 
     async def modify_db_proxy_endpoint(
         self,
         *,
         DBProxyEndpointName: str,
         NewDBProxyEndpointName: str = ...,
-        VpcSecurityGroupIds: Sequence[str] = ...
+        VpcSecurityGroupIds: Sequence[str] = ...,
     ) -> ModifyDBProxyEndpointResponseTypeDef:
         """
         Changes the settings for an existing DB proxy endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_proxy_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_proxy_endpoint)
         """
 
     async def modify_db_proxy_target_group(
         self,
         *,
         TargetGroupName: str,
         DBProxyName: str,
         ConnectionPoolConfig: ConnectionPoolConfigurationTypeDef = ...,
-        NewName: str = ...
+        NewName: str = ...,
     ) -> ModifyDBProxyTargetGroupResponseTypeDef:
         """
         Modifies the properties of a `DBProxyTargetGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_proxy_target_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_proxy_target_group)
         """
@@ -2369,15 +2369,15 @@
 
     async def modify_db_snapshot_attribute(
         self,
         *,
         DBSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual DB
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_snapshot_attribute)
@@ -2385,15 +2385,15 @@
         """
 
     async def modify_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         SubnetIds: Sequence[str],
-        DBSubnetGroupDescription: str = ...
+        DBSubnetGroupDescription: str = ...,
     ) -> ModifyDBSubnetGroupResultTypeDef:
         """
         Modifies an existing DB subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_subnet_group)
         """
@@ -2401,15 +2401,15 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing RDS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_event_subscription)
         """
@@ -2417,59 +2417,59 @@
     async def modify_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
-        AllowMajorVersionUpgrade: bool = ...
+        AllowMajorVersionUpgrade: bool = ...,
     ) -> ModifyGlobalClusterResultTypeDef:
         """
         Modifies a setting for an Amazon Aurora global database cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_global_cluster)
         """
 
     async def modify_option_group(
         self,
         *,
         OptionGroupName: str,
         OptionsToInclude: Sequence[OptionConfigurationTypeDef] = ...,
         OptionsToRemove: Sequence[str] = ...,
-        ApplyImmediately: bool = ...
+        ApplyImmediately: bool = ...,
     ) -> ModifyOptionGroupResultTypeDef:
         """
         Modifies an existing option group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_option_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_option_group)
         """
 
     async def modify_tenant_database(
         self,
         *,
         DBInstanceIdentifier: str,
         TenantDBName: str,
         MasterUserPassword: str = ...,
-        NewTenantDBName: str = ...
+        NewTenantDBName: str = ...,
     ) -> ModifyTenantDatabaseResultTypeDef:
         """
         Modifies an existing tenant database in a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_tenant_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_tenant_database)
         """
 
     async def promote_read_replica(
         self,
         *,
         DBInstanceIdentifier: str,
         BackupRetentionPeriod: int = ...,
-        PreferredBackupWindow: str = ...
+        PreferredBackupWindow: str = ...,
     ) -> PromoteReadReplicaResultTypeDef:
         """
         Promotes a read replica DB instance to a standalone DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.promote_read_replica)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#promote_read_replica)
         """
@@ -2486,15 +2486,15 @@
 
     async def purchase_reserved_db_instances_offering(
         self,
         *,
         ReservedDBInstancesOfferingId: str,
         ReservedDBInstanceId: str = ...,
         DBInstanceCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PurchaseReservedDBInstancesOfferingResultTypeDef:
         """
         Purchases a reserved DB instance offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.purchase_reserved_db_instances_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#purchase_reserved_db_instances_offering)
         """
@@ -2519,15 +2519,15 @@
 
     async def register_db_proxy_targets(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         DBInstanceIdentifiers: Sequence[str] = ...,
-        DBClusterIdentifiers: Sequence[str] = ...
+        DBClusterIdentifiers: Sequence[str] = ...,
     ) -> RegisterDBProxyTargetsResponseTypeDef:
         """
         Associate one or more `DBProxyTarget` data structures with a
         `DBProxyTargetGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.register_db_proxy_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#register_db_proxy_targets)
@@ -2589,29 +2589,29 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_cluster_parameter_group)
         """
 
     async def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_parameter_group)
@@ -2651,15 +2651,15 @@
         CopyTagsToSnapshot: bool = ...,
         Domain: str = ...,
         DomainIAMRoleName: str = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterFromS3ResultTypeDef:
         """
         Creates an Amazon Aurora DB cluster from MySQL data stored in an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_from_s3)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_from_s3)
@@ -2692,15 +2692,15 @@
         DomainIAMRoleName: str = ...,
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         Iops: int = ...,
         PubliclyAccessible: bool = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
-        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...
+        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...,
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new DB cluster from a DB snapshot or DB cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_from_snapshot)
         """
@@ -2732,15 +2732,15 @@
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         PubliclyAccessible: bool = ...,
         Iops: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         SourceDbClusterResourceId: str = ...,
-        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...
+        RdsCustomClusterConfiguration: RdsCustomClusterConfigurationTypeDef = ...,
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_to_point_in_time)
         """
@@ -2783,15 +2783,15 @@
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         DBClusterSnapshotIdentifier: str = ...,
         AllocatedStorage: int = ...,
-        DedicatedLogVolume: bool = ...
+        DedicatedLogVolume: bool = ...,
     ) -> RestoreDBInstanceFromDBSnapshotResultTypeDef:
         """
         Creates a new DB instance from a DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_db_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_instance_from_db_snapshot)
         """
@@ -2843,15 +2843,15 @@
         UseDefaultProcessorFeatures: bool = ...,
         DeletionProtection: bool = ...,
         MaxAllocatedStorage: int = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        DedicatedLogVolume: bool = ...
+        DedicatedLogVolume: bool = ...,
     ) -> RestoreDBInstanceFromS3ResultTypeDef:
         """
         Amazon Relational Database Service (Amazon RDS) supports importing MySQL
         databases by using backup
         files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_s3)
@@ -2900,15 +2900,15 @@
         SourceDBInstanceAutomatedBackupsArn: str = ...,
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         AllocatedStorage: int = ...,
-        DedicatedLogVolume: bool = ...
+        DedicatedLogVolume: bool = ...,
     ) -> RestoreDBInstanceToPointInTimeResultTypeDef:
         """
         Restores a DB instance to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_instance_to_point_in_time)
         """
@@ -2916,15 +2916,15 @@
     async def revoke_db_security_group_ingress(
         self,
         *,
         DBSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupId: str = ...,
-        EC2SecurityGroupOwnerId: str = ...
+        EC2SecurityGroupOwnerId: str = ...,
     ) -> RevokeDBSecurityGroupIngressResultTypeDef:
         """
         Revokes ingress from a DBSecurityGroup for previously authorized IP ranges or
         EC2 or VPC security
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.revoke_db_security_group_ingress)
@@ -2934,15 +2934,15 @@
     async def start_activity_stream(
         self,
         *,
         ResourceArn: str,
         Mode: ActivityStreamModeType,
         KmsKeyId: str,
         ApplyImmediately: bool = ...,
-        EngineNativeAuditFieldsIncluded: bool = ...
+        EngineNativeAuditFieldsIncluded: bool = ...,
     ) -> StartActivityStreamResponseTypeDef:
         """
         Starts a database activity stream to monitor activity on the database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_activity_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#start_activity_stream)
         """
@@ -2970,15 +2970,15 @@
     async def start_db_instance_automated_backups_replication(
         self,
         *,
         SourceDBInstanceArn: str,
         BackupRetentionPeriod: int = ...,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> StartDBInstanceAutomatedBackupsReplicationResultTypeDef:
         """
         Enables replication of automated backups to a different Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_db_instance_automated_backups_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#start_db_instance_automated_backups_replication)
@@ -2989,15 +2989,15 @@
         *,
         ExportTaskIdentifier: str,
         SourceArn: str,
         S3BucketName: str,
         IamRoleArn: str,
         KmsKeyId: str,
         S3Prefix: str = ...,
-        ExportOnly: Sequence[str] = ...
+        ExportOnly: Sequence[str] = ...,
     ) -> ExportTaskResponseTypeDef:
         """
         Starts an export of DB snapshot or DB cluster data to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.start_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#start_export_task)
         """
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/literals.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/literals.py`

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
     "ActivityStreamModeType",
     "ActivityStreamPolicyStatusType",
     "ActivityStreamStatusType",
     "ApplyMethodType",
     "AuditPolicyStateType",
     "AuthSchemeType",
@@ -101,15 +100,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActivityStreamModeType = Literal["async", "sync"]
 ActivityStreamPolicyStatusType = Literal["locked", "locking-policy", "unlocked", "unlocking-policy"]
 ActivityStreamStatusType = Literal["started", "starting", "stopped", "stopping"]
 ApplyMethodType = Literal["immediate", "pending-reboot"]
 AuditPolicyStateType = Literal["locked", "unlocked"]
 AuthSchemeType = Literal["SECRETS"]
 AutomationModeType = Literal["all-paused", "full"]
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/literals.pyi` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/paginator.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,14 @@
     "DescribeReservedDBInstancesPaginator",
     "DescribeReservedDBInstancesOfferingsPaginator",
     "DescribeSourceRegionsPaginator",
     "DescribeTenantDatabasesPaginator",
     "DownloadDBLogFilePortionPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -208,15 +207,15 @@
     """
 
     def paginate(
         self,
         *,
         BlueGreenDeploymentIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBlueGreenDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeBlueGreenDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describebluegreendeploymentspaginator)
         """
 
 
@@ -227,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describecertificatespaginator)
         """
 
 
@@ -247,15 +246,15 @@
 
     def paginate(
         self,
         *,
         DbClusterResourceId: str = ...,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterAutomatedBackupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterAutomatedBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterautomatedbackupspaginator)
         """
 
 
@@ -267,15 +266,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterBacktrackMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterBacktracks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterbacktrackspaginator)
         """
 
 
@@ -287,15 +286,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterendpointspaginator)
         """
 
 
@@ -306,15 +305,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterparametergroupspaginator)
         """
 
 
@@ -326,15 +325,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterparameterspaginator)
         """
 
 
@@ -350,15 +349,15 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbClusterResourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclustersnapshotspaginator)
         """
 
 
@@ -370,15 +369,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterspaginator)
         """
 
 
@@ -395,15 +394,15 @@
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
         IncludeAll: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbengineversionspaginator)
         """
 
 
@@ -416,15 +415,15 @@
     def paginate(
         self,
         *,
         DbiResourceId: str = ...,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DBInstanceAutomatedBackupsArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceAutomatedBackupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBInstanceAutomatedBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbinstanceautomatedbackupspaginator)
         """
 
 
@@ -435,15 +434,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbinstancespaginator)
         """
 
 
@@ -457,15 +456,15 @@
         self,
         *,
         DBInstanceIdentifier: str,
         FilenameContains: str = ...,
         FileLastWritten: int = ...,
         FileSize: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBLogFilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBLogFiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedblogfilespaginator)
         """
 
 
@@ -476,15 +475,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbparametergroupspaginator)
         """
 
 
@@ -496,15 +495,15 @@
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbparameterspaginator)
         """
 
 
@@ -515,15 +514,15 @@
     """
 
     def paginate(
         self,
         *,
         DBProxyName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxiespaginator)
         """
 
 
@@ -535,15 +534,15 @@
 
     def paginate(
         self,
         *,
         DBProxyName: str = ...,
         DBProxyEndpointName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxyEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxyendpointspaginator)
         """
 
 
@@ -555,15 +554,15 @@
 
     def paginate(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxyTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxytargetgroupspaginator)
         """
 
 
@@ -575,15 +574,15 @@
 
     def paginate(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxyTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxytargetspaginator)
         """
 
 
@@ -594,15 +593,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSecurityGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsecuritygroupspaginator)
         """
 
 
@@ -616,15 +615,15 @@
         self,
         *,
         DBInstanceIdentifier: str = ...,
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DbiResourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSnapshotTenantDatabasesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSnapshotTenantDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsnapshottenantdatabasespaginator)
         """
 
 
@@ -640,15 +639,15 @@
         DBInstanceIdentifier: str = ...,
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsnapshotspaginator)
         """
 
 
@@ -659,15 +658,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsubnetgroupspaginator)
         """
 
 
@@ -678,15 +677,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEngineDefaultClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeenginedefaultclusterparameterspaginator)
         """
 
 
@@ -697,15 +696,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeenginedefaultparameterspaginator)
         """
 
 
@@ -716,15 +715,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -740,15 +739,15 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeeventspaginator)
         """
 
 
@@ -761,15 +760,15 @@
     def paginate(
         self,
         *,
         ExportTaskIdentifier: str = ...,
         SourceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SourceType: ExportSourceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ExportTasksMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeexporttaskspaginator)
         """
 
 
@@ -780,15 +779,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeglobalclusterspaginator)
         """
 
 
@@ -799,15 +798,15 @@
     """
 
     def paginate(
         self,
         *,
         IntegrationIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeIntegrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeintegrationspaginator)
         """
 
 
@@ -819,15 +818,15 @@
 
     def paginate(
         self,
         *,
         EngineName: str,
         MajorEngineVersion: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OptionGroupOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOptionGroupOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeoptiongroupoptionspaginator)
         """
 
 
@@ -840,15 +839,15 @@
     def paginate(
         self,
         *,
         OptionGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         EngineName: str = ...,
         MajorEngineVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OptionGroupsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOptionGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeoptiongroupspaginator)
         """
 
 
@@ -864,15 +863,15 @@
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         AvailabilityZoneGroup: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 
@@ -883,15 +882,15 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describependingmaintenanceactionspaginator)
         """
 
 
@@ -909,15 +908,15 @@
         DBInstanceClass: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         LeaseId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedDBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeReservedDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describereserveddbinstancespaginator)
         """
 
 
@@ -933,15 +932,15 @@
         ReservedDBInstancesOfferingId: str = ...,
         DBInstanceClass: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedDBInstancesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeReservedDBInstancesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describereserveddbinstancesofferingspaginator)
         """
 
 
@@ -952,15 +951,15 @@
     """
 
     def paginate(
         self,
         *,
         RegionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SourceRegionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeSourceRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describesourceregionspaginator)
         """
 
 
@@ -972,15 +971,15 @@
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TenantDatabasesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeTenantDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describetenantdatabasespaginator)
         """
 
 
@@ -991,13 +990,13 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str,
         LogFileName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DownloadDBLogFilePortionDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DownloadDBLogFilePortion.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#downloaddblogfileportionpaginator)
         """
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/paginator.pyi` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     """
 
     def paginate(
         self,
         *,
         BlueGreenDeploymentIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBlueGreenDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeBlueGreenDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describebluegreendeploymentspaginator)
         """
 
 class DescribeCertificatesPaginator(AioPaginator):
@@ -223,15 +223,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describecertificatespaginator)
         """
 
 class DescribeDBClusterAutomatedBackupsPaginator(AioPaginator):
@@ -242,15 +242,15 @@
 
     def paginate(
         self,
         *,
         DbClusterResourceId: str = ...,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterAutomatedBackupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterAutomatedBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterautomatedbackupspaginator)
         """
 
 class DescribeDBClusterBacktracksPaginator(AioPaginator):
@@ -261,15 +261,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterBacktrackMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterBacktracks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterbacktrackspaginator)
         """
 
 class DescribeDBClusterEndpointsPaginator(AioPaginator):
@@ -280,15 +280,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterendpointspaginator)
         """
 
 class DescribeDBClusterParameterGroupsPaginator(AioPaginator):
@@ -298,15 +298,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterparametergroupspaginator)
         """
 
 class DescribeDBClusterParametersPaginator(AioPaginator):
@@ -317,15 +317,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterparameterspaginator)
         """
 
 class DescribeDBClusterSnapshotsPaginator(AioPaginator):
@@ -340,15 +340,15 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbClusterResourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclustersnapshotspaginator)
         """
 
 class DescribeDBClustersPaginator(AioPaginator):
@@ -359,15 +359,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclusterspaginator)
         """
 
 class DescribeDBEngineVersionsPaginator(AioPaginator):
@@ -383,15 +383,15 @@
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
         IncludeAll: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbengineversionspaginator)
         """
 
 class DescribeDBInstanceAutomatedBackupsPaginator(AioPaginator):
@@ -403,15 +403,15 @@
     def paginate(
         self,
         *,
         DbiResourceId: str = ...,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DBInstanceAutomatedBackupsArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceAutomatedBackupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBInstanceAutomatedBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbinstanceautomatedbackupspaginator)
         """
 
 class DescribeDBInstancesPaginator(AioPaginator):
@@ -421,15 +421,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbinstancespaginator)
         """
 
 class DescribeDBLogFilesPaginator(AioPaginator):
@@ -442,15 +442,15 @@
         self,
         *,
         DBInstanceIdentifier: str,
         FilenameContains: str = ...,
         FileLastWritten: int = ...,
         FileSize: int = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBLogFilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBLogFiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedblogfilespaginator)
         """
 
 class DescribeDBParameterGroupsPaginator(AioPaginator):
@@ -460,15 +460,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbparametergroupspaginator)
         """
 
 class DescribeDBParametersPaginator(AioPaginator):
@@ -479,15 +479,15 @@
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbparameterspaginator)
         """
 
 class DescribeDBProxiesPaginator(AioPaginator):
@@ -497,15 +497,15 @@
     """
 
     def paginate(
         self,
         *,
         DBProxyName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxiespaginator)
         """
 
 class DescribeDBProxyEndpointsPaginator(AioPaginator):
@@ -516,15 +516,15 @@
 
     def paginate(
         self,
         *,
         DBProxyName: str = ...,
         DBProxyEndpointName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxyEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxyendpointspaginator)
         """
 
 class DescribeDBProxyTargetGroupsPaginator(AioPaginator):
@@ -535,15 +535,15 @@
 
     def paginate(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxyTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxytargetgroupspaginator)
         """
 
 class DescribeDBProxyTargetsPaginator(AioPaginator):
@@ -554,15 +554,15 @@
 
     def paginate(
         self,
         *,
         DBProxyName: str,
         TargetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDBProxyTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBProxyTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbproxytargetspaginator)
         """
 
 class DescribeDBSecurityGroupsPaginator(AioPaginator):
@@ -572,15 +572,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSecurityGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsecuritygroupspaginator)
         """
 
 class DescribeDBSnapshotTenantDatabasesPaginator(AioPaginator):
@@ -593,15 +593,15 @@
         self,
         *,
         DBInstanceIdentifier: str = ...,
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DbiResourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSnapshotTenantDatabasesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSnapshotTenantDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsnapshottenantdatabasespaginator)
         """
 
 class DescribeDBSnapshotsPaginator(AioPaginator):
@@ -616,15 +616,15 @@
         DBInstanceIdentifier: str = ...,
         DBSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsnapshotspaginator)
         """
 
 class DescribeDBSubnetGroupsPaginator(AioPaginator):
@@ -634,15 +634,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbsubnetgroupspaginator)
         """
 
 class DescribeEngineDefaultClusterParametersPaginator(AioPaginator):
@@ -652,15 +652,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEngineDefaultClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeenginedefaultclusterparameterspaginator)
         """
 
 class DescribeEngineDefaultParametersPaginator(AioPaginator):
@@ -670,15 +670,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeenginedefaultparameterspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -688,15 +688,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -711,15 +711,15 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeeventspaginator)
         """
 
 class DescribeExportTasksPaginator(AioPaginator):
@@ -731,15 +731,15 @@
     def paginate(
         self,
         *,
         ExportTaskIdentifier: str = ...,
         SourceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SourceType: ExportSourceTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ExportTasksMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeexporttaskspaginator)
         """
 
 class DescribeGlobalClustersPaginator(AioPaginator):
@@ -749,15 +749,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeglobalclusterspaginator)
         """
 
 class DescribeIntegrationsPaginator(AioPaginator):
@@ -767,15 +767,15 @@
     """
 
     def paginate(
         self,
         *,
         IntegrationIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeIntegrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeintegrationspaginator)
         """
 
 class DescribeOptionGroupOptionsPaginator(AioPaginator):
@@ -786,15 +786,15 @@
 
     def paginate(
         self,
         *,
         EngineName: str,
         MajorEngineVersion: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OptionGroupOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOptionGroupOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeoptiongroupoptionspaginator)
         """
 
 class DescribeOptionGroupsPaginator(AioPaginator):
@@ -806,15 +806,15 @@
     def paginate(
         self,
         *,
         OptionGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         EngineName: str = ...,
         MajorEngineVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OptionGroupsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOptionGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeoptiongroupspaginator)
         """
 
 class DescribeOrderableDBInstanceOptionsPaginator(AioPaginator):
@@ -829,15 +829,15 @@
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         AvailabilityZoneGroup: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 class DescribePendingMaintenanceActionsPaginator(AioPaginator):
@@ -847,15 +847,15 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describependingmaintenanceactionspaginator)
         """
 
 class DescribeReservedDBInstancesPaginator(AioPaginator):
@@ -872,15 +872,15 @@
         DBInstanceClass: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         LeaseId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedDBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeReservedDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describereserveddbinstancespaginator)
         """
 
 class DescribeReservedDBInstancesOfferingsPaginator(AioPaginator):
@@ -895,15 +895,15 @@
         ReservedDBInstancesOfferingId: str = ...,
         DBInstanceClass: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
         MultiAZ: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ReservedDBInstancesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeReservedDBInstancesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describereserveddbinstancesofferingspaginator)
         """
 
 class DescribeSourceRegionsPaginator(AioPaginator):
@@ -913,15 +913,15 @@
     """
 
     def paginate(
         self,
         *,
         RegionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SourceRegionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeSourceRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describesourceregionspaginator)
         """
 
 class DescribeTenantDatabasesPaginator(AioPaginator):
@@ -932,15 +932,15 @@
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[TenantDatabasesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeTenantDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describetenantdatabasespaginator)
         """
 
 class DownloadDBLogFilePortionPaginator(AioPaginator):
@@ -950,13 +950,13 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str,
         LogFileName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DownloadDBLogFilePortionDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DownloadDBLogFilePortion.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#downloaddblogfileportionpaginator)
         """
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/type_defs.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountQuotaTypeDef",
     "ResponseMetadataTypeDef",
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddRoleToDBInstanceMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/type_defs.pyi` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/waiter.py` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,59 +57,56 @@
     "DBSnapshotAvailableWaiter",
     "DBSnapshotCompletedWaiter",
     "DBSnapshotDeletedWaiter",
     "TenantDatabaseAvailableWaiter",
     "TenantDatabaseDeletedWaiter",
 )
 
-
 class DBClusterAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusteravailablewaiter)
     """
 
     async def wait(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusteravailablewaiter)
         """
 
-
 class DBClusterDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusterdeletedwaiter)
     """
 
     async def wait(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusterdeletedwaiter)
         """
 
-
 class DBClusterSnapshotAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotavailablewaiter)
     """
 
     async def wait(
@@ -120,22 +117,21 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbClusterResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotavailablewaiter)
         """
 
-
 class DBClusterSnapshotDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotdeletedwaiter)
     """
 
     async def wait(
@@ -146,64 +142,61 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbClusterResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotdeletedwaiter)
         """
 
-
 class DBInstanceAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstanceavailablewaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstanceavailablewaiter)
         """
 
-
 class DBInstanceDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstancedeletedwaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstancedeletedwaiter)
         """
 
-
 class DBSnapshotAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotavailablewaiter)
     """
 
     async def wait(
@@ -214,22 +207,21 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotavailablewaiter)
         """
 
-
 class DBSnapshotCompletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotCompleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotcompletedwaiter)
     """
 
     async def wait(
@@ -240,22 +232,21 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotCompleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotcompletedwaiter)
         """
 
-
 class DBSnapshotDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotdeletedwaiter)
     """
 
     async def wait(
@@ -266,57 +257,55 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotdeletedwaiter)
         """
 
-
 class TenantDatabaseAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabaseavailablewaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabaseavailablewaiter)
         """
 
-
 class TenantDatabaseDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabasedeletedwaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabasedeletedwaiter)
         """
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds/waiter.pyi` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds/waiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,56 +57,59 @@
     "DBSnapshotAvailableWaiter",
     "DBSnapshotCompletedWaiter",
     "DBSnapshotDeletedWaiter",
     "TenantDatabaseAvailableWaiter",
     "TenantDatabaseDeletedWaiter",
 )
 
+
 class DBClusterAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusteravailablewaiter)
     """
 
     async def wait(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusteravailablewaiter)
         """
 
+
 class DBClusterDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusterdeletedwaiter)
     """
 
     async def wait(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclusterdeletedwaiter)
         """
 
+
 class DBClusterSnapshotAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotavailablewaiter)
     """
 
     async def wait(
@@ -117,21 +120,22 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbClusterResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotavailablewaiter)
         """
 
+
 class DBClusterSnapshotDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotdeletedwaiter)
     """
 
     async def wait(
@@ -142,61 +146,64 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbClusterResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotdeletedwaiter)
         """
 
+
 class DBInstanceAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstanceavailablewaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstanceavailablewaiter)
         """
 
+
 class DBInstanceDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstancedeletedwaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbinstancedeletedwaiter)
         """
 
+
 class DBSnapshotAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotavailablewaiter)
     """
 
     async def wait(
@@ -207,21 +214,22 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotavailablewaiter)
         """
 
+
 class DBSnapshotCompletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotCompleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotcompletedwaiter)
     """
 
     async def wait(
@@ -232,21 +240,22 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotCompleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotcompletedwaiter)
         """
 
+
 class DBSnapshotDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotdeletedwaiter)
     """
 
     async def wait(
@@ -257,55 +266,57 @@
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
         DbiResourceId: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBSnapshotDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbsnapshotdeletedwaiter)
         """
 
+
 class TenantDatabaseAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabaseavailablewaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabaseavailablewaiter)
         """
 
+
 class TenantDatabaseDeletedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseDeleted)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabasedeletedwaiter)
     """
 
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         TenantDBName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.TenantDatabaseDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#tenantdatabasedeletedwaiter)
         """
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/PKG-INFO` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RDS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RDS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/
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
 
 <a id="types-aiobotocore-rds"></a>
 
 # types-aiobotocore-rds
 
 [![PyPI - types-aiobotocore-rds](https://img.shields.io/pypi/v/types-aiobotocore-rds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rds)](https://pepy.tech/project/types-aiobotocore-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[aiobotocore.RDS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [types-aiobotocore-rds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rds-2.9.0/types_aiobotocore_rds.egg-info/SOURCES.txt` & `types-aiobotocore-rds-2.9.1/types_aiobotocore_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

