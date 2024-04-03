# Comparing `tmp/types-aiobotocore-dms-2.9.0.tar.gz` & `tmp/types-aiobotocore-dms-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dms-2.9.0.tar", last modified: Wed Dec 13 19:59:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-dms-2.9.1.tar", last modified: Thu Jan 18 01:20:32 2024, max compression
```

## Comparing `types-aiobotocore-dms-2.9.0.tar` & `types-aiobotocore-dms-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.565826 types-aiobotocore-dms-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17064 2023-12-13 19:59:07.565826 types-aiobotocore-dms-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:07.565826 types-aiobotocore-dms-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.561826 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98066 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    98062 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15867 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17807 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   135554 2023-12-13 19:44:18.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   135553 2023-12-13 19:44:17.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:14.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10051 2023-12-13 19:44:15.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:07.565826 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17064 2023-12-13 19:59:07.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:07.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:07.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:07.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:07.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:07.000000 types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.889381 types-aiobotocore-dms-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17084 2024-01-18 01:20:32.889381 types-aiobotocore-dms-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:32.889381 types-aiobotocore-dms-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.889381 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98108 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98105 2024-01-18 01:06:09.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15867 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15867 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   135553 2024-01-18 01:06:13.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135553 2024-01-18 01:06:12.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:08.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-01-18 01:06:10.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.889381 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17084 2024-01-18 01:20:32.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:32.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:32.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:32.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:32.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:32.000000 types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dms-2.9.0/LICENSE` & `types-aiobotocore-dms-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-dms-2.9.0/PKG-INFO` & `types-aiobotocore-dms-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
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
 
 <a id="types-aiobotocore-dms"></a>
 
 # types-aiobotocore-dms
 
 [![PyPI - types-aiobotocore-dms](https://img.shields.io/pypi/v/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [types-aiobotocore-dms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dms-2.9.0/README.md` & `types-aiobotocore-dms-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [types-aiobotocore-dms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dms-2.9.0/setup.py` & `types-aiobotocore-dms-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dms",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DatabaseMigrationService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DatabaseMigrationService 2.9.1 service generated with"
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
     keywords="aiobotocore dms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dms": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/__init__.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     ReplicationTaskRunningWaiter,
     ReplicationTaskStoppedWaiter,
     TestConnectionSucceedsWaiter,
 )
 
 Client = DatabaseMigrationServiceClient
 
-
 __all__ = (
     "Client",
     "DatabaseMigrationServiceClient",
     "DescribeCertificatesPaginator",
     "DescribeConnectionsPaginator",
     "DescribeEndpointTypesPaginator",
     "DescribeEndpointsPaginator",
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/__init__.pyi` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/__main__.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DatabaseMigrationService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DatabaseMigrationService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/client.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DatabaseMigrationServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -318,15 +317,15 @@
     async def create_data_provider(
         self,
         *,
         Engine: str,
         Settings: DataProviderSettingsTypeDef,
         DataProviderName: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataProviderResponseTypeDef:
         """
         Creates a data provider using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_data_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_data_provider)
         """
@@ -364,15 +363,15 @@
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
-        TimestreamSettings: TimestreamSettingsTypeDef = ...
+        TimestreamSettings: TimestreamSettingsTypeDef = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_endpoint)
         """
@@ -382,30 +381,30 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResponseTypeDef:
         """
         Creates an DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_event_subscription)
         """
 
     async def create_fleet_advisor_collector(
         self,
         *,
         CollectorName: str,
         ServiceAccessRoleArn: str,
         S3BucketName: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateFleetAdvisorCollectorResponseTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_fleet_advisor_collector)
         """
@@ -417,15 +416,15 @@
         KmsKeyArn: str = ...,
         PubliclyAccessible: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         NetworkType: str = ...,
         InstanceProfileName: str = ...,
         Description: str = ...,
         SubnetGroupIdentifier: str = ...,
-        VpcSecurityGroups: Sequence[str] = ...
+        VpcSecurityGroups: Sequence[str] = ...,
     ) -> CreateInstanceProfileResponseTypeDef:
         """
         Creates the instance profile using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_instance_profile)
         """
@@ -436,15 +435,15 @@
         SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],
         TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],
         InstanceProfileIdentifier: str,
         MigrationProjectName: str = ...,
         TransformationRules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...
+        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...,
     ) -> CreateMigrationProjectResponseTypeDef:
         """
         Creates the migration project using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_migration_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_migration_project)
         """
@@ -457,15 +456,15 @@
         TargetEndpointArn: str,
         ComputeConfig: ComputeConfigTypeDef,
         ReplicationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ResourceIdentifier: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateReplicationConfigResponseTypeDef:
         """
         Creates a configuration that you can later provide to configure and start an
         DMS Serverless
         replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
@@ -486,30 +485,30 @@
         EngineVersion: str = ...,
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         PubliclyAccessible: bool = ...,
         DnsNameServers: str = ...,
         ResourceIdentifier: str = ...,
-        NetworkType: str = ...
+        NetworkType: str = ...,
     ) -> CreateReplicationInstanceResponseTypeDef:
         """
         Creates the replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_instance)
         """
 
     async def create_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         ReplicationSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateReplicationSubnetGroupResponseTypeDef:
         """
         Creates a replication subnet group given a list of the subnet IDs in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_subnet_group)
         """
@@ -525,15 +524,15 @@
         TableMappings: str,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
-        ResourceIdentifier: str = ...
+        ResourceIdentifier: str = ...,
     ) -> CreateReplicationTaskResponseTypeDef:
         """
         Creates a replication task using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_task)
         """
@@ -687,15 +686,15 @@
         *,
         ReplicationTaskArn: str = ...,
         ReplicationInstanceArn: str = ...,
         SourceEngineName: str = ...,
         TargetEngineName: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:
         """
         Provides a list of individual assessments that you can specify for a new
         premigration assessment run, given one or more
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_applicable_individual_assessments)
@@ -801,15 +800,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEventSubscriptionsResponseTypeDef:
         """
         Lists all the event subscriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_event_subscriptions)
         """
@@ -821,30 +820,30 @@
         SourceType: Literal["replication-instance"] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEventsResponseTypeDef:
         """
         Lists events for a given source identifier and source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_events)
         """
 
     async def describe_extension_pack_associations(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeExtensionPackAssociationsResponseTypeDef:
         """
         Returns a paginated list of extension pack associations for the specified
         migration
         project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_extension_pack_associations)
@@ -917,15 +916,15 @@
 
     async def describe_metadata_model_assessments(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelAssessmentsResponseTypeDef:
         """
         Returns a paginated list of metadata model assessments for your account in the
         current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_assessments)
@@ -934,60 +933,60 @@
 
     async def describe_metadata_model_conversions(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelConversionsResponseTypeDef:
         """
         Returns a paginated list of metadata model conversions for a migration project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_conversions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_conversions)
         """
 
     async def describe_metadata_model_exports_as_script(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelExportsAsScriptResponseTypeDef:
         """
         Returns a paginated list of metadata model exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_exports_as_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_exports_as_script)
         """
 
     async def describe_metadata_model_exports_to_target(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelExportsToTargetResponseTypeDef:
         """
         Returns a paginated list of metadata model exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_exports_to_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_exports_to_target)
         """
 
     async def describe_metadata_model_imports(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelImportsResponseTypeDef:
         """
         Returns a paginated list of metadata model imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_imports)
         """
@@ -1017,15 +1016,15 @@
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ReplicationInstanceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribePendingMaintenanceActionsResponseTypeDef:
         """
         For internal use only See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/dms-2016-01-01/DescribePendingMaintenanceActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_pending_maintenance_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_pending_maintenance_actions)
@@ -1109,15 +1108,15 @@
 
     async def describe_replication_table_statistics(
         self,
         *,
         ReplicationConfigArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> DescribeReplicationTableStatisticsResponseTypeDef:
         """
         Returns table and schema statistics for one or more provisioned replications
         that use a given DMS Serverless replication
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
@@ -1159,15 +1158,15 @@
 
     async def describe_replication_tasks(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WithoutSettings: bool = ...
+        WithoutSettings: bool = ...,
     ) -> DescribeReplicationTasksResponseTypeDef:
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_tasks)
@@ -1197,15 +1196,15 @@
 
     async def describe_table_statistics(
         self,
         *,
         ReplicationTaskArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> DescribeTableStatisticsResponseTypeDef:
         """
         Returns table statistics on the database migration task, including table name,
         rows inserted, rows updated, and rows
         deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_table_statistics)
@@ -1214,15 +1213,15 @@
 
     async def export_metadata_model_assessment(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
         FileName: str = ...,
-        AssessmentReportTypes: Sequence[AssessmentReportTypeType] = ...
+        AssessmentReportTypes: Sequence[AssessmentReportTypeType] = ...,
     ) -> ExportMetadataModelAssessmentResponseTypeDef:
         """
         Saves a copy of a database migration assessment report to your Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.export_metadata_model_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#export_metadata_model_assessment)
         """
@@ -1243,15 +1242,15 @@
 
     async def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
         CertificateWallet: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#import_certificate)
         """
@@ -1283,15 +1282,15 @@
         self,
         *,
         DataProviderIdentifier: str,
         DataProviderName: str = ...,
         Description: str = ...,
         Engine: str = ...,
         ExactSettings: bool = ...,
-        Settings: DataProviderSettingsTypeDef = ...
+        Settings: DataProviderSettingsTypeDef = ...,
     ) -> ModifyDataProviderResponseTypeDef:
         """
         Modifies the specified data provider using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_data_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_data_provider)
         """
@@ -1328,15 +1327,15 @@
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
-        TimestreamSettings: TimestreamSettingsTypeDef = ...
+        TimestreamSettings: TimestreamSettingsTypeDef = ...,
     ) -> ModifyEndpointResponseTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_endpoint)
         """
@@ -1344,15 +1343,15 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResponseTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_event_subscription)
         """
@@ -1364,15 +1363,15 @@
         AvailabilityZone: str = ...,
         KmsKeyArn: str = ...,
         PubliclyAccessible: bool = ...,
         NetworkType: str = ...,
         InstanceProfileName: str = ...,
         Description: str = ...,
         SubnetGroupIdentifier: str = ...,
-        VpcSecurityGroups: Sequence[str] = ...
+        VpcSecurityGroups: Sequence[str] = ...,
     ) -> ModifyInstanceProfileResponseTypeDef:
         """
         Modifies the specified instance profile using the provided parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_instance_profile)
         """
@@ -1383,15 +1382,15 @@
         MigrationProjectIdentifier: str,
         MigrationProjectName: str = ...,
         SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef] = ...,
         TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef] = ...,
         InstanceProfileIdentifier: str = ...,
         TransformationRules: str = ...,
         Description: str = ...,
-        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...
+        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...,
     ) -> ModifyMigrationProjectResponseTypeDef:
         """
         Modifies the specified migration project using the provided parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_migration_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_migration_project)
         """
@@ -1403,15 +1402,15 @@
         ReplicationConfigIdentifier: str = ...,
         ReplicationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ComputeConfig: ComputeConfigTypeDef = ...,
         SourceEndpointArn: str = ...,
-        TargetEndpointArn: str = ...
+        TargetEndpointArn: str = ...,
     ) -> ModifyReplicationConfigResponseTypeDef:
         """
         Modifies an existing DMS Serverless replication configuration that you can use
         to start a
         replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
@@ -1428,29 +1427,29 @@
         VpcSecurityGroupIds: Sequence[str] = ...,
         PreferredMaintenanceWindow: str = ...,
         MultiAZ: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         AutoMinorVersionUpgrade: bool = ...,
         ReplicationInstanceIdentifier: str = ...,
-        NetworkType: str = ...
+        NetworkType: str = ...,
     ) -> ModifyReplicationInstanceResponseTypeDef:
         """
         Modifies the replication instance to apply new settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_instance)
         """
 
     async def modify_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         SubnetIds: Sequence[str],
-        ReplicationSubnetGroupDescription: str = ...
+        ReplicationSubnetGroupDescription: str = ...,
     ) -> ModifyReplicationSubnetGroupResponseTypeDef:
         """
         Modifies the settings for the specified replication subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_subnet_group)
         """
@@ -1462,15 +1461,15 @@
         ReplicationTaskIdentifier: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
-        TaskData: str = ...
+        TaskData: str = ...,
     ) -> ModifyReplicationTaskResponseTypeDef:
         """
         Modifies the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_task)
         """
@@ -1488,15 +1487,15 @@
         """
 
     async def reboot_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         ForceFailover: bool = ...,
-        ForcePlannedFailover: bool = ...
+        ForcePlannedFailover: bool = ...,
     ) -> RebootReplicationInstanceResponseTypeDef:
         """
         Reboots a replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reboot_replication_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#reboot_replication_instance)
         """
@@ -1512,15 +1511,15 @@
         """
 
     async def reload_replication_tables(
         self,
         *,
         ReplicationConfigArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
-        ReloadOption: ReloadOptionValueType = ...
+        ReloadOption: ReloadOptionValueType = ...,
     ) -> ReloadReplicationTablesResponseTypeDef:
         """
         Reloads the target database table with the source data for a given DMS
         Serverless replication
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
@@ -1528,15 +1527,15 @@
         """
 
     async def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
-        ReloadOption: ReloadOptionValueType = ...
+        ReloadOption: ReloadOptionValueType = ...,
     ) -> ReloadTablesResponseTypeDef:
         """
         Reloads the target database table with the source data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#reload_tables)
         """
@@ -1598,15 +1597,15 @@
 
     async def start_metadata_model_export_as_script(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
         Origin: OriginTypeValueType,
-        FileName: str = ...
+        FileName: str = ...,
     ) -> StartMetadataModelExportAsScriptResponseTypeDef:
         """
         Saves your converted code to a file as a SQL script, and stores this file on
         your Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_metadata_model_export_as_script)
@@ -1614,30 +1613,30 @@
         """
 
     async def start_metadata_model_export_to_target(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
-        OverwriteExtensionPack: bool = ...
+        OverwriteExtensionPack: bool = ...,
     ) -> StartMetadataModelExportToTargetResponseTypeDef:
         """
         Applies converted database objects to your target database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_metadata_model_export_to_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_metadata_model_export_to_target)
         """
 
     async def start_metadata_model_import(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
         Origin: OriginTypeValueType,
-        Refresh: bool = ...
+        Refresh: bool = ...,
     ) -> StartMetadataModelImportResponseTypeDef:
         """
         Loads the metadata for all the dependent database objects of the parent object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_metadata_model_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_metadata_model_import)
         """
@@ -1657,15 +1656,15 @@
     async def start_replication(
         self,
         *,
         ReplicationConfigArn: str,
         StartReplicationType: str,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
-        CdcStopPosition: str = ...
+        CdcStopPosition: str = ...,
     ) -> StartReplicationResponseTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS connects to the
         source endpoint and collects the metadata to analyze the replication
         workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
@@ -1675,15 +1674,15 @@
     async def start_replication_task(
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
-        CdcStopPosition: str = ...
+        CdcStopPosition: str = ...,
     ) -> StartReplicationTaskResponseTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_replication_task)
         """
@@ -1706,15 +1705,15 @@
         ServiceAccessRoleArn: str,
         ResultLocationBucket: str,
         AssessmentRunName: str,
         ResultLocationFolder: str = ...,
         ResultEncryptionMode: str = ...,
         ResultKmsKeyArn: str = ...,
         IncludeOnly: Sequence[str] = ...,
-        Exclude: Sequence[str] = ...
+        Exclude: Sequence[str] = ...,
     ) -> StartReplicationTaskAssessmentRunResponseTypeDef:
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/client.pyi` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     async def create_data_provider(
         self,
         *,
         Engine: str,
         Settings: DataProviderSettingsTypeDef,
         DataProviderName: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataProviderResponseTypeDef:
         """
         Creates a data provider using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_data_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_data_provider)
         """
@@ -360,15 +360,15 @@
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
-        TimestreamSettings: TimestreamSettingsTypeDef = ...
+        TimestreamSettings: TimestreamSettingsTypeDef = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_endpoint)
         """
@@ -378,30 +378,30 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResponseTypeDef:
         """
         Creates an DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_event_subscription)
         """
 
     async def create_fleet_advisor_collector(
         self,
         *,
         CollectorName: str,
         ServiceAccessRoleArn: str,
         S3BucketName: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateFleetAdvisorCollectorResponseTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_fleet_advisor_collector)
         """
@@ -413,15 +413,15 @@
         KmsKeyArn: str = ...,
         PubliclyAccessible: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         NetworkType: str = ...,
         InstanceProfileName: str = ...,
         Description: str = ...,
         SubnetGroupIdentifier: str = ...,
-        VpcSecurityGroups: Sequence[str] = ...
+        VpcSecurityGroups: Sequence[str] = ...,
     ) -> CreateInstanceProfileResponseTypeDef:
         """
         Creates the instance profile using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_instance_profile)
         """
@@ -432,15 +432,15 @@
         SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],
         TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef],
         InstanceProfileIdentifier: str,
         MigrationProjectName: str = ...,
         TransformationRules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...
+        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...,
     ) -> CreateMigrationProjectResponseTypeDef:
         """
         Creates the migration project using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_migration_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_migration_project)
         """
@@ -453,15 +453,15 @@
         TargetEndpointArn: str,
         ComputeConfig: ComputeConfigTypeDef,
         ReplicationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ResourceIdentifier: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateReplicationConfigResponseTypeDef:
         """
         Creates a configuration that you can later provide to configure and start an
         DMS Serverless
         replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
@@ -482,30 +482,30 @@
         EngineVersion: str = ...,
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         PubliclyAccessible: bool = ...,
         DnsNameServers: str = ...,
         ResourceIdentifier: str = ...,
-        NetworkType: str = ...
+        NetworkType: str = ...,
     ) -> CreateReplicationInstanceResponseTypeDef:
         """
         Creates the replication instance using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_instance)
         """
 
     async def create_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         ReplicationSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateReplicationSubnetGroupResponseTypeDef:
         """
         Creates a replication subnet group given a list of the subnet IDs in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_subnet_group)
         """
@@ -521,15 +521,15 @@
         TableMappings: str,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
-        ResourceIdentifier: str = ...
+        ResourceIdentifier: str = ...,
     ) -> CreateReplicationTaskResponseTypeDef:
         """
         Creates a replication task using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_task)
         """
@@ -683,15 +683,15 @@
         *,
         ReplicationTaskArn: str = ...,
         ReplicationInstanceArn: str = ...,
         SourceEngineName: str = ...,
         TargetEngineName: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeApplicableIndividualAssessmentsResponseTypeDef:
         """
         Provides a list of individual assessments that you can specify for a new
         premigration assessment run, given one or more
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_applicable_individual_assessments)
@@ -797,15 +797,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEventSubscriptionsResponseTypeDef:
         """
         Lists all the event subscriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_event_subscriptions)
         """
@@ -817,30 +817,30 @@
         SourceType: Literal["replication-instance"] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEventsResponseTypeDef:
         """
         Lists events for a given source identifier and source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_events)
         """
 
     async def describe_extension_pack_associations(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeExtensionPackAssociationsResponseTypeDef:
         """
         Returns a paginated list of extension pack associations for the specified
         migration
         project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_extension_pack_associations)
@@ -913,15 +913,15 @@
 
     async def describe_metadata_model_assessments(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelAssessmentsResponseTypeDef:
         """
         Returns a paginated list of metadata model assessments for your account in the
         current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_assessments)
@@ -930,60 +930,60 @@
 
     async def describe_metadata_model_conversions(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelConversionsResponseTypeDef:
         """
         Returns a paginated list of metadata model conversions for a migration project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_conversions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_conversions)
         """
 
     async def describe_metadata_model_exports_as_script(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelExportsAsScriptResponseTypeDef:
         """
         Returns a paginated list of metadata model exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_exports_as_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_exports_as_script)
         """
 
     async def describe_metadata_model_exports_to_target(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelExportsToTargetResponseTypeDef:
         """
         Returns a paginated list of metadata model exports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_exports_to_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_exports_to_target)
         """
 
     async def describe_metadata_model_imports(
         self,
         *,
         MigrationProjectIdentifier: str,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribeMetadataModelImportsResponseTypeDef:
         """
         Returns a paginated list of metadata model imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_metadata_model_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_metadata_model_imports)
         """
@@ -1013,15 +1013,15 @@
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ReplicationInstanceArn: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> DescribePendingMaintenanceActionsResponseTypeDef:
         """
         For internal use only See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/dms-2016-01-01/DescribePendingMaintenanceActions).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_pending_maintenance_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_pending_maintenance_actions)
@@ -1105,15 +1105,15 @@
 
     async def describe_replication_table_statistics(
         self,
         *,
         ReplicationConfigArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> DescribeReplicationTableStatisticsResponseTypeDef:
         """
         Returns table and schema statistics for one or more provisioned replications
         that use a given DMS Serverless replication
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
@@ -1155,15 +1155,15 @@
 
     async def describe_replication_tasks(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WithoutSettings: bool = ...
+        WithoutSettings: bool = ...,
     ) -> DescribeReplicationTasksResponseTypeDef:
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_tasks)
@@ -1193,15 +1193,15 @@
 
     async def describe_table_statistics(
         self,
         *,
         ReplicationTaskArn: str,
         MaxRecords: int = ...,
         Marker: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> DescribeTableStatisticsResponseTypeDef:
         """
         Returns table statistics on the database migration task, including table name,
         rows inserted, rows updated, and rows
         deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_table_statistics)
@@ -1210,15 +1210,15 @@
 
     async def export_metadata_model_assessment(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
         FileName: str = ...,
-        AssessmentReportTypes: Sequence[AssessmentReportTypeType] = ...
+        AssessmentReportTypes: Sequence[AssessmentReportTypeType] = ...,
     ) -> ExportMetadataModelAssessmentResponseTypeDef:
         """
         Saves a copy of a database migration assessment report to your Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.export_metadata_model_assessment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#export_metadata_model_assessment)
         """
@@ -1239,15 +1239,15 @@
 
     async def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
         CertificateWallet: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#import_certificate)
         """
@@ -1279,15 +1279,15 @@
         self,
         *,
         DataProviderIdentifier: str,
         DataProviderName: str = ...,
         Description: str = ...,
         Engine: str = ...,
         ExactSettings: bool = ...,
-        Settings: DataProviderSettingsTypeDef = ...
+        Settings: DataProviderSettingsTypeDef = ...,
     ) -> ModifyDataProviderResponseTypeDef:
         """
         Modifies the specified data provider using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_data_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_data_provider)
         """
@@ -1324,15 +1324,15 @@
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
-        TimestreamSettings: TimestreamSettingsTypeDef = ...
+        TimestreamSettings: TimestreamSettingsTypeDef = ...,
     ) -> ModifyEndpointResponseTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_endpoint)
         """
@@ -1340,15 +1340,15 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResponseTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_event_subscription)
         """
@@ -1360,15 +1360,15 @@
         AvailabilityZone: str = ...,
         KmsKeyArn: str = ...,
         PubliclyAccessible: bool = ...,
         NetworkType: str = ...,
         InstanceProfileName: str = ...,
         Description: str = ...,
         SubnetGroupIdentifier: str = ...,
-        VpcSecurityGroups: Sequence[str] = ...
+        VpcSecurityGroups: Sequence[str] = ...,
     ) -> ModifyInstanceProfileResponseTypeDef:
         """
         Modifies the specified instance profile using the provided parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_instance_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_instance_profile)
         """
@@ -1379,15 +1379,15 @@
         MigrationProjectIdentifier: str,
         MigrationProjectName: str = ...,
         SourceDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef] = ...,
         TargetDataProviderDescriptors: Sequence[DataProviderDescriptorDefinitionTypeDef] = ...,
         InstanceProfileIdentifier: str = ...,
         TransformationRules: str = ...,
         Description: str = ...,
-        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...
+        SchemaConversionApplicationAttributes: SCApplicationAttributesTypeDef = ...,
     ) -> ModifyMigrationProjectResponseTypeDef:
         """
         Modifies the specified migration project using the provided parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_migration_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_migration_project)
         """
@@ -1399,15 +1399,15 @@
         ReplicationConfigIdentifier: str = ...,
         ReplicationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationSettings: str = ...,
         SupplementalSettings: str = ...,
         ComputeConfig: ComputeConfigTypeDef = ...,
         SourceEndpointArn: str = ...,
-        TargetEndpointArn: str = ...
+        TargetEndpointArn: str = ...,
     ) -> ModifyReplicationConfigResponseTypeDef:
         """
         Modifies an existing DMS Serverless replication configuration that you can use
         to start a
         replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
@@ -1424,29 +1424,29 @@
         VpcSecurityGroupIds: Sequence[str] = ...,
         PreferredMaintenanceWindow: str = ...,
         MultiAZ: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         AutoMinorVersionUpgrade: bool = ...,
         ReplicationInstanceIdentifier: str = ...,
-        NetworkType: str = ...
+        NetworkType: str = ...,
     ) -> ModifyReplicationInstanceResponseTypeDef:
         """
         Modifies the replication instance to apply new settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_instance)
         """
 
     async def modify_replication_subnet_group(
         self,
         *,
         ReplicationSubnetGroupIdentifier: str,
         SubnetIds: Sequence[str],
-        ReplicationSubnetGroupDescription: str = ...
+        ReplicationSubnetGroupDescription: str = ...,
     ) -> ModifyReplicationSubnetGroupResponseTypeDef:
         """
         Modifies the settings for the specified replication subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_subnet_group)
         """
@@ -1458,15 +1458,15 @@
         ReplicationTaskIdentifier: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
-        TaskData: str = ...
+        TaskData: str = ...,
     ) -> ModifyReplicationTaskResponseTypeDef:
         """
         Modifies the specified replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_task)
         """
@@ -1484,15 +1484,15 @@
         """
 
     async def reboot_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         ForceFailover: bool = ...,
-        ForcePlannedFailover: bool = ...
+        ForcePlannedFailover: bool = ...,
     ) -> RebootReplicationInstanceResponseTypeDef:
         """
         Reboots a replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reboot_replication_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#reboot_replication_instance)
         """
@@ -1508,15 +1508,15 @@
         """
 
     async def reload_replication_tables(
         self,
         *,
         ReplicationConfigArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
-        ReloadOption: ReloadOptionValueType = ...
+        ReloadOption: ReloadOptionValueType = ...,
     ) -> ReloadReplicationTablesResponseTypeDef:
         """
         Reloads the target database table with the source data for a given DMS
         Serverless replication
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
@@ -1524,15 +1524,15 @@
         """
 
     async def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
-        ReloadOption: ReloadOptionValueType = ...
+        ReloadOption: ReloadOptionValueType = ...,
     ) -> ReloadTablesResponseTypeDef:
         """
         Reloads the target database table with the source data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#reload_tables)
         """
@@ -1594,15 +1594,15 @@
 
     async def start_metadata_model_export_as_script(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
         Origin: OriginTypeValueType,
-        FileName: str = ...
+        FileName: str = ...,
     ) -> StartMetadataModelExportAsScriptResponseTypeDef:
         """
         Saves your converted code to a file as a SQL script, and stores this file on
         your Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_metadata_model_export_as_script)
@@ -1610,30 +1610,30 @@
         """
 
     async def start_metadata_model_export_to_target(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
-        OverwriteExtensionPack: bool = ...
+        OverwriteExtensionPack: bool = ...,
     ) -> StartMetadataModelExportToTargetResponseTypeDef:
         """
         Applies converted database objects to your target database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_metadata_model_export_to_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_metadata_model_export_to_target)
         """
 
     async def start_metadata_model_import(
         self,
         *,
         MigrationProjectIdentifier: str,
         SelectionRules: str,
         Origin: OriginTypeValueType,
-        Refresh: bool = ...
+        Refresh: bool = ...,
     ) -> StartMetadataModelImportResponseTypeDef:
         """
         Loads the metadata for all the dependent database objects of the parent object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_metadata_model_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_metadata_model_import)
         """
@@ -1653,15 +1653,15 @@
     async def start_replication(
         self,
         *,
         ReplicationConfigArn: str,
         StartReplicationType: str,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
-        CdcStopPosition: str = ...
+        CdcStopPosition: str = ...,
     ) -> StartReplicationResponseTypeDef:
         """
         For a given DMS Serverless replication configuration, DMS connects to the
         source endpoint and collects the metadata to analyze the replication
         workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
@@ -1671,15 +1671,15 @@
     async def start_replication_task(
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
-        CdcStopPosition: str = ...
+        CdcStopPosition: str = ...,
     ) -> StartReplicationTaskResponseTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_replication_task)
         """
@@ -1702,15 +1702,15 @@
         ServiceAccessRoleArn: str,
         ResultLocationBucket: str,
         AssessmentRunName: str,
         ResultLocationFolder: str = ...,
         ResultEncryptionMode: str = ...,
         ResultKmsKeyArn: str = ...,
         IncludeOnly: Sequence[str] = ...,
-        Exclude: Sequence[str] = ...
+        Exclude: Sequence[str] = ...,
     ) -> StartReplicationTaskAssessmentRunResponseTypeDef:
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration
         task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/literals.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/literals.py`

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
     "AssessmentReportTypeType",
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
@@ -83,15 +82,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AssessmentReportTypeType = Literal["csv", "pdf"]
 AuthMechanismValueType = Literal["default", "mongodb_cr", "scram_sha_1"]
 AuthTypeValueType = Literal["no", "password"]
 CannedAclForObjectsValueType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/literals.pyi` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/paginator.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeCertificatesPaginator",
     "DescribeConnectionsPaginator",
     "DescribeEndpointTypesPaginator",
     "DescribeEndpointsPaginator",
     "DescribeEventSubscriptionsPaginator",
     "DescribeEventsPaginator",
@@ -88,15 +87,14 @@
     "DescribeReplicationSubnetGroupsPaginator",
     "DescribeReplicationTaskAssessmentResultsPaginator",
     "DescribeReplicationTasksPaginator",
     "DescribeSchemasPaginator",
     "DescribeTableStatisticsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -109,15 +107,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
         """
 
 
@@ -127,15 +125,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
         """
 
 
@@ -145,15 +143,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
         """
 
 
@@ -163,15 +161,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEndpointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
         """
 
 
@@ -182,15 +180,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -206,15 +204,15 @@
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventspaginator)
         """
 
 
@@ -239,15 +237,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
         """
 
 
@@ -257,15 +255,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 
@@ -291,15 +289,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskspaginator)
         """
 
 
@@ -325,13 +323,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/paginator.pyi` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
         """
 
 class DescribeConnectionsPaginator(AioPaginator):
@@ -122,15 +122,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
         """
 
 class DescribeEndpointTypesPaginator(AioPaginator):
@@ -139,15 +139,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
         """
 
 class DescribeEndpointsPaginator(AioPaginator):
@@ -156,15 +156,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEndpointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -174,15 +174,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -197,15 +197,15 @@
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventspaginator)
         """
 
 class DescribeOrderableReplicationInstancesPaginator(AioPaginator):
@@ -228,15 +228,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
         """
 
 class DescribeReplicationSubnetGroupsPaginator(AioPaginator):
@@ -245,15 +245,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 class DescribeReplicationTaskAssessmentResultsPaginator(AioPaginator):
@@ -277,15 +277,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskspaginator)
         """
 
 class DescribeSchemasPaginator(AioPaginator):
@@ -309,13 +309,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/type_defs.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/type_defs.pyi` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/waiter.py` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.EndpointDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#endpointdeletedwaiter)
         """
 
 
@@ -81,15 +81,15 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationinstanceavailablewaiter)
         """
 
 
@@ -101,15 +101,15 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationinstancedeletedwaiter)
         """
 
 
@@ -122,15 +122,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskdeletedwaiter)
         """
 
 
@@ -143,15 +143,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskReady.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskreadywaiter)
         """
 
 
@@ -164,15 +164,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskrunningwaiter)
         """
 
 
@@ -185,15 +185,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskstoppedwaiter)
         """
 
 
@@ -205,13 +205,13 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.TestConnectionSucceeds.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#testconnectionsucceedswaiter)
         """
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms/waiter.pyi` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms/waiter.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.EndpointDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#endpointdeletedwaiter)
         """
 
 class ReplicationInstanceAvailableWaiter(AIOWaiter):
@@ -79,15 +79,15 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationinstanceavailablewaiter)
         """
 
 class ReplicationInstanceDeletedWaiter(AIOWaiter):
@@ -98,15 +98,15 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationinstancedeletedwaiter)
         """
 
 class ReplicationTaskDeletedWaiter(AIOWaiter):
@@ -118,15 +118,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskdeletedwaiter)
         """
 
 class ReplicationTaskReadyWaiter(AIOWaiter):
@@ -138,15 +138,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskReady.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskreadywaiter)
         """
 
 class ReplicationTaskRunningWaiter(AIOWaiter):
@@ -158,15 +158,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskrunningwaiter)
         """
 
 class ReplicationTaskStoppedWaiter(AIOWaiter):
@@ -178,15 +178,15 @@
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         WithoutSettings: bool = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.ReplicationTaskStopped.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#replicationtaskstoppedwaiter)
         """
 
 class TestConnectionSucceedsWaiter(AIOWaiter):
@@ -197,13 +197,13 @@
 
     async def wait(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Waiter.TestConnectionSucceeds.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/waiters/#testconnectionsucceedswaiter)
         """
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/PKG-INFO` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
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
 
 <a id="types-aiobotocore-dms"></a>
 
 # types-aiobotocore-dms
 
 [![PyPI - types-aiobotocore-dms](https://img.shields.io/pypi/v/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [types-aiobotocore-dms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dms-2.9.0/types_aiobotocore_dms.egg-info/SOURCES.txt` & `types-aiobotocore-dms-2.9.1/types_aiobotocore_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

