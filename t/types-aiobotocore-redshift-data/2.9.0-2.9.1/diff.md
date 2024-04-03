# Comparing `tmp/types-aiobotocore-redshift-data-2.9.0.tar.gz` & `tmp/types-aiobotocore-redshift-data-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-data-2.9.0.tar", last modified: Wed Dec 13 20:00:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-data-2.9.1.tar", last modified: Thu Jan 18 01:21:35 2024, max compression
```

## Comparing `types-aiobotocore-redshift-data-2.9.0.tar` & `types-aiobotocore-redshift-data-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.853264 types-aiobotocore-redshift-data-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2023-12-13 20:00:15.853264 types-aiobotocore-redshift-data-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:15.853264 types-aiobotocore-redshift-data-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.849264 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2023-12-13 19:54:26.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2023-12-13 19:54:26.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2023-12-13 19:54:26.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2023-12-13 19:54:26.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2023-12-13 19:54:26.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13783 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13782 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:25.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:15.853264 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2023-12-13 20:00:15.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 20:00:15.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:15.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:15.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:15.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 20:00:15.000000 types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.585093 types-aiobotocore-redshift-data-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-01-18 01:21:35.585093 types-aiobotocore-redshift-data-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:35.585093 types-aiobotocore-redshift-data-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-01-18 01:16:03.000000 types-aiobotocore-redshift-data-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.585093 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8728 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:04.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:35.585093 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:35.000000 types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/LICENSE` & `types-aiobotocore-redshift-data-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-redshift-data-2.9.0/PKG-INFO` & `types-aiobotocore-redshift-data-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
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
 
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-data)](https://pepy.tech/project/types-aiobotocore-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftDataAPIService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[aiobotocore.RedshiftDataAPIService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/README.md` & `types-aiobotocore-redshift-data-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-data)](https://pepy.tech/project/types-aiobotocore-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftDataAPIService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[aiobotocore.RedshiftDataAPIService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/setup.py` & `types-aiobotocore-redshift-data-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-data",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RedshiftDataAPIService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.RedshiftDataAPIService 2.9.1 service generated with"
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
     keywords="aiobotocore redshift-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_redshift_data": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/__init__.py` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListSchemasPaginator,
     ListStatementsPaginator,
     ListTablesPaginator,
 )
 
 Client = RedshiftDataAPIServiceClient
 
-
 __all__ = (
     "Client",
     "DescribeTablePaginator",
     "GetStatementResultPaginator",
     "ListDatabasesPaginator",
     "ListSchemasPaginator",
     "ListStatementsPaginator",
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/__init__.pyi` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/__main__.py` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RedshiftDataAPIService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RedshiftDataAPIService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
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

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/client.py` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RedshiftDataAPIServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -96,15 +95,15 @@
         Sqls: Sequence[str],
         ClientToken: str = ...,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         StatementName: str = ...,
         WithEvent: bool = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> BatchExecuteStatementOutputTypeDef:
         """
         Runs one or more SQL statements, which can be data manipulation language (DML)
         or data definition language
         (DDL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.batch_execute_statement)
@@ -153,15 +152,15 @@
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> DescribeTableResponseTypeDef:
         """
         Describes the detailed information about a table from metadata in the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.describe_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#describe_table)
         """
@@ -174,15 +173,15 @@
         ClientToken: str = ...,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         Parameters: Sequence[SqlParameterTypeDef] = ...,
         SecretArn: str = ...,
         StatementName: str = ...,
         WithEvent: bool = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ExecuteStatementOutputTypeDef:
         """
         Runs an SQL statement, which can be data manipulation language (DML) or data
         definition language
         (DDL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.execute_statement)
@@ -218,15 +217,15 @@
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SecretArn: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ListDatabasesResponseTypeDef:
         """
         List the databases in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_databases)
         """
@@ -238,15 +237,15 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ListSchemasResponseTypeDef:
         """
         Lists the schemas in a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_schemas)
         """
@@ -254,15 +253,15 @@
     async def list_statements(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         RoleLevel: bool = ...,
         StatementName: str = ...,
-        Status: StatusStringType = ...
+        Status: StatusStringType = ...,
     ) -> ListStatementsResponseTypeDef:
         """
         List of SQL statements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_statements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_statements)
         """
@@ -275,15 +274,15 @@
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ListTablesResponseTypeDef:
         """
         List the tables in a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_tables)
         """
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/client.pyi` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         Sqls: Sequence[str],
         ClientToken: str = ...,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         StatementName: str = ...,
         WithEvent: bool = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> BatchExecuteStatementOutputTypeDef:
         """
         Runs one or more SQL statements, which can be data manipulation language (DML)
         or data definition language
         (DDL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.batch_execute_statement)
@@ -149,15 +149,15 @@
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> DescribeTableResponseTypeDef:
         """
         Describes the detailed information about a table from metadata in the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.describe_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#describe_table)
         """
@@ -170,15 +170,15 @@
         ClientToken: str = ...,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         Parameters: Sequence[SqlParameterTypeDef] = ...,
         SecretArn: str = ...,
         StatementName: str = ...,
         WithEvent: bool = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ExecuteStatementOutputTypeDef:
         """
         Runs an SQL statement, which can be data manipulation language (DML) or data
         definition language
         (DDL).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.execute_statement)
@@ -214,15 +214,15 @@
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SecretArn: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ListDatabasesResponseTypeDef:
         """
         List the databases in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_databases)
         """
@@ -234,15 +234,15 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ListSchemasResponseTypeDef:
         """
         Lists the schemas in a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_schemas)
         """
@@ -250,15 +250,15 @@
     async def list_statements(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         RoleLevel: bool = ...,
         StatementName: str = ...,
-        Status: StatusStringType = ...
+        Status: StatusStringType = ...,
     ) -> ListStatementsResponseTypeDef:
         """
         List of SQL statements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_statements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_statements)
         """
@@ -271,15 +271,15 @@
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
-        WorkgroupName: str = ...
+        WorkgroupName: str = ...,
     ) -> ListTablesResponseTypeDef:
         """
         List the tables in a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.list_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/client/#list_tables)
         """
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/literals.py` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/literals.py`

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
     "DescribeTablePaginatorName",
     "GetStatementResultPaginatorName",
     "ListDatabasesPaginatorName",
     "ListSchemasPaginatorName",
     "ListStatementsPaginatorName",
     "ListTablesPaginatorName",
@@ -31,15 +30,14 @@
     "StatusStringType",
     "RedshiftDataAPIServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DescribeTablePaginatorName = Literal["describe_table"]
 GetStatementResultPaginatorName = Literal["get_statement_result"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 ListStatementsPaginatorName = Literal["list_statements"]
 ListTablesPaginatorName = Literal["list_tables"]
 StatementStatusStringType = Literal[
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/literals.pyi` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/paginator.py` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "GetStatementResultPaginator",
     "ListDatabasesPaginator",
     "ListSchemasPaginator",
     "ListStatementsPaginator",
     "ListTablesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -80,15 +79,15 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#describetablepaginator)
         """
 
 
@@ -117,15 +116,15 @@
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listdatabasespaginator)
         """
 
 
@@ -141,15 +140,15 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listschemaspaginator)
         """
 
 
@@ -161,15 +160,15 @@
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#liststatementspaginator)
         """
 
 
@@ -186,13 +185,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/paginator.pyi` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#describetablepaginator)
         """
 
 class GetStatementResultPaginator(AioPaginator):
@@ -112,15 +112,15 @@
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listdatabasespaginator)
         """
 
 class ListSchemasPaginator(AioPaginator):
@@ -135,15 +135,15 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listschemaspaginator)
         """
 
 class ListStatementsPaginator(AioPaginator):
@@ -154,15 +154,15 @@
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#liststatementspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
@@ -178,13 +178,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/type_defs.py` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
     "SqlParameterTypeDef",
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data/type_defs.pyi` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/PKG-INFO` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
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
 
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-data)](https://pepy.tech/project/types-aiobotocore-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftDataAPIService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[aiobotocore.RedshiftDataAPIService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-data-2.9.0/types_aiobotocore_redshift_data.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-data-2.9.1/types_aiobotocore_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

