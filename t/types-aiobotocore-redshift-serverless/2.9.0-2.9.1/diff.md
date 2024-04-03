# Comparing `tmp/types-aiobotocore-redshift-serverless-2.9.0.tar.gz` & `tmp/types-aiobotocore-redshift-serverless-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-serverless-2.9.0.tar", last modified: Wed Dec 13 20:00:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-serverless-2.9.1.tar", last modified: Thu Jan 18 01:21:36 2024, max compression
```

## Comparing `types-aiobotocore-redshift-serverless-2.9.0.tar` & `types-aiobotocore-redshift-serverless-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:16.629258 types-aiobotocore-redshift-serverless-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15150 2023-12-13 20:00:16.629258 types-aiobotocore-redshift-serverless-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13540 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:16.629258 types-aiobotocore-redshift-serverless-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:16.629258 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48549 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48545 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13850 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    45072 2023-12-13 19:54:31.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45071 2023-12-13 19:54:30.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:29.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:16.629258 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15150 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:16.000000 types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:36.309090 types-aiobotocore-redshift-serverless-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-01-18 01:21:36.309090 types-aiobotocore-redshift-serverless-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13540 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:36.309090 types-aiobotocore-redshift-serverless-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:36.309090 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48571 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48568 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45071 2024-01-18 01:16:06.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45071 2024-01-18 01:16:06.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:05.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:36.309090 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-01-18 01:21:36.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-18 01:21:36.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:36.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:36.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:36.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:36.000000 types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/LICENSE` & `types-aiobotocore-redshift-serverless-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/PKG-INFO` & `types-aiobotocore-redshift-serverless-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-serverless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RedshiftServerless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RedshiftServerless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/
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
 
 <a id="types-aiobotocore-redshift-serverless"></a>
 
 # types-aiobotocore-redshift-serverless
 
 [![PyPI - types-aiobotocore-redshift-serverless](https://img.shields.io/pypi/v/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[aiobotocore.RedshiftServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [types-aiobotocore-redshift-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/README.md` & `types-aiobotocore-redshift-serverless-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[aiobotocore.RedshiftServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [types-aiobotocore-redshift-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/setup.py` & `types-aiobotocore-redshift-serverless-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-serverless",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RedshiftServerless 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.RedshiftServerless 2.9.1 service generated with"
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
     keywords="aiobotocore redshift-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_redshift_serverless": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/__init__.py` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListTableRestoreStatusPaginator,
     ListUsageLimitsPaginator,
     ListWorkgroupsPaginator,
 )
 
 Client = RedshiftServerlessClient
 
-
 __all__ = (
     "Client",
     "ListCustomDomainAssociationsPaginator",
     "ListEndpointAccessPaginator",
     "ListNamespacesPaginator",
     "ListRecoveryPointsPaginator",
     "ListScheduledActionsPaginator",
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/__init__.pyi` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/__main__.py` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RedshiftServerless 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RedshiftServerless 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/client.py` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RedshiftServerlessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -164,15 +163,15 @@
 
     async def convert_recovery_point_to_snapshot(
         self,
         *,
         recoveryPointId: str,
         snapshotName: str,
         retentionPeriod: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ConvertRecoveryPointToSnapshotResponseTypeDef:
         """
         Converts a recovery point to a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.convert_recovery_point_to_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#convert_recovery_point_to_snapshot)
         """
@@ -190,15 +189,15 @@
     async def create_endpoint_access(
         self,
         *,
         endpointName: str,
         subnetIds: Sequence[str],
         workgroupName: str,
         ownerAccount: str = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> CreateEndpointAccessResponseTypeDef:
         """
         Creates an Amazon Redshift Serverless managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_endpoint_access)
         """
@@ -213,15 +212,15 @@
         dbName: str = ...,
         defaultIamRoleArn: str = ...,
         iamRoles: Sequence[str] = ...,
         kmsKeyId: str = ...,
         logExports: Sequence[LogExportType] = ...,
         manageAdminPassword: bool = ...,
         redshiftIdcApplicationArn: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNamespaceResponseTypeDef:
         """
         Creates a namespace in Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_namespace)
         """
@@ -233,45 +232,45 @@
         roleArn: str,
         schedule: ScheduleTypeDef,
         scheduledActionName: str,
         targetAction: TargetActionTypeDef,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         scheduledActionDescription: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> CreateScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_scheduled_action)
         """
 
     async def create_snapshot(
         self,
         *,
         namespaceName: str,
         snapshotName: str,
         retentionPeriod: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a snapshot of all databases in a namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_snapshot)
         """
 
     async def create_snapshot_copy_configuration(
         self,
         *,
         destinationRegion: str,
         namespaceName: str,
         destinationKmsKeyId: str = ...,
-        snapshotRetentionPeriod: int = ...
+        snapshotRetentionPeriod: int = ...,
     ) -> CreateSnapshotCopyConfigurationResponseTypeDef:
         """
         Creates a snapshot copy configuration that lets you copy snapshots to another
         Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_snapshot_copy_configuration)
@@ -281,15 +280,15 @@
     async def create_usage_limit(
         self,
         *,
         amount: int,
         resourceArn: str,
         usageType: UsageLimitUsageTypeType,
         breachAction: UsageLimitBreachActionType = ...,
-        period: UsageLimitPeriodType = ...
+        period: UsageLimitPeriodType = ...,
     ) -> CreateUsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift Serverless usage type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_usage_limit)
         """
@@ -303,15 +302,15 @@
         configParameters: Sequence[ConfigParameterTypeDef] = ...,
         enhancedVpcRouting: bool = ...,
         maxCapacity: int = ...,
         port: int = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkgroupResponseTypeDef:
         """
         Creates an workgroup in Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_workgroup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_workgroup)
         """
@@ -337,15 +336,15 @@
         """
 
     async def delete_namespace(
         self,
         *,
         namespaceName: str,
         finalSnapshotName: str = ...,
-        finalSnapshotRetentionPeriod: int = ...
+        finalSnapshotRetentionPeriod: int = ...,
     ) -> DeleteNamespaceResponseTypeDef:
         """
         Deletes a namespace from Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.delete_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#delete_namespace)
         """
@@ -419,15 +418,15 @@
 
     async def get_credentials(
         self,
         *,
         customDomainName: str = ...,
         dbName: str = ...,
         durationSeconds: int = ...,
-        workgroupName: str = ...
+        workgroupName: str = ...,
     ) -> GetCredentialsResponseTypeDef:
         """
         Returns a database user name and temporary password with temporary
         authorization to log in to Amazon Redshift
         Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.get_credentials)
@@ -524,15 +523,15 @@
 
     async def list_custom_domain_associations(
         self,
         *,
         customDomainCertificateArn: str = ...,
         customDomainName: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCustomDomainAssociationsResponseTypeDef:
         """
         Lists custom domain associations for Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_custom_domain_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_custom_domain_associations)
         """
@@ -540,15 +539,15 @@
     async def list_endpoint_access(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
         vpcId: str = ...,
-        workgroupName: str = ...
+        workgroupName: str = ...,
     ) -> ListEndpointAccessResponseTypeDef:
         """
         Returns an array of `EndpointAccess` objects and relevant information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_endpoint_access)
         """
@@ -567,15 +566,15 @@
         self,
         *,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListRecoveryPointsResponseTypeDef:
         """
         Returns an array of recovery points.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_recovery_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_recovery_points)
         """
@@ -605,30 +604,30 @@
         *,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListSnapshotsResponseTypeDef:
         """
         Returns a list of snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_snapshots)
         """
 
     async def list_table_restore_status(
         self,
         *,
         maxResults: int = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        workgroupName: str = ...
+        workgroupName: str = ...,
     ) -> ListTableRestoreStatusResponseTypeDef:
         """
         Returns information about an array of `TableRestoreStatus` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_table_restore_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_table_restore_status)
         """
@@ -645,15 +644,15 @@
 
     async def list_usage_limits(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         resourceArn: str = ...,
-        usageType: UsageLimitUsageTypeType = ...
+        usageType: UsageLimitUsageTypeType = ...,
     ) -> ListUsageLimitsResponseTypeDef:
         """
         Lists all usage limits within Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_usage_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_usage_limits)
         """
@@ -693,15 +692,15 @@
         *,
         namespaceName: str,
         workgroupName: str,
         adminPasswordSecretKmsKeyId: str = ...,
         manageAdminPassword: bool = ...,
         ownerAccount: str = ...,
         snapshotArn: str = ...,
-        snapshotName: str = ...
+        snapshotName: str = ...,
     ) -> RestoreFromSnapshotResponseTypeDef:
         """
         Restores a namespace from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.restore_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#restore_from_snapshot)
         """
@@ -714,15 +713,15 @@
         recoveryPointId: str,
         sourceDatabaseName: str,
         sourceTableName: str,
         workgroupName: str,
         activateCaseSensitiveIdentifier: bool = ...,
         sourceSchemaName: str = ...,
         targetDatabaseName: str = ...,
-        targetSchemaName: str = ...
+        targetSchemaName: str = ...,
     ) -> RestoreTableFromRecoveryPointResponseTypeDef:
         """
         Restores a table from a recovery point to your Amazon Redshift Serverless
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.restore_table_from_recovery_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#restore_table_from_recovery_point)
@@ -736,15 +735,15 @@
         snapshotName: str,
         sourceDatabaseName: str,
         sourceTableName: str,
         workgroupName: str,
         activateCaseSensitiveIdentifier: bool = ...,
         sourceSchemaName: str = ...,
         targetDatabaseName: str = ...,
-        targetSchemaName: str = ...
+        targetSchemaName: str = ...,
     ) -> RestoreTableFromSnapshotResponseTypeDef:
         """
         Restores a table from a snapshot to your Amazon Redshift Serverless instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.restore_table_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#restore_table_from_snapshot)
         """
@@ -793,15 +792,15 @@
         adminPasswordSecretKmsKeyId: str = ...,
         adminUserPassword: str = ...,
         adminUsername: str = ...,
         defaultIamRoleArn: str = ...,
         iamRoles: Sequence[str] = ...,
         kmsKeyId: str = ...,
         logExports: Sequence[LogExportType] = ...,
-        manageAdminPassword: bool = ...
+        manageAdminPassword: bool = ...,
     ) -> UpdateNamespaceResponseTypeDef:
         """
         Updates a namespace with the specified settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_namespace)
         """
@@ -812,15 +811,15 @@
         scheduledActionName: str,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         roleArn: str = ...,
         schedule: ScheduleTypeDef = ...,
         scheduledActionDescription: str = ...,
         startTime: TimestampTypeDef = ...,
-        targetAction: TargetActionTypeDef = ...
+        targetAction: TargetActionTypeDef = ...,
     ) -> UpdateScheduledActionResponseTypeDef:
         """
         Updates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_scheduled_action)
         """
@@ -846,15 +845,15 @@
         """
 
     async def update_usage_limit(
         self,
         *,
         usageLimitId: str,
         amount: int = ...,
-        breachAction: UsageLimitBreachActionType = ...
+        breachAction: UsageLimitBreachActionType = ...,
     ) -> UpdateUsageLimitResponseTypeDef:
         """
         Update a usage limit in Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_usage_limit)
         """
@@ -866,15 +865,15 @@
         baseCapacity: int = ...,
         configParameters: Sequence[ConfigParameterTypeDef] = ...,
         enhancedVpcRouting: bool = ...,
         maxCapacity: int = ...,
         port: int = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
-        subnetIds: Sequence[str] = ...
+        subnetIds: Sequence[str] = ...,
     ) -> UpdateWorkgroupResponseTypeDef:
         """
         Updates a workgroup with the specified configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_workgroup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_workgroup)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/client.pyi` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
     async def convert_recovery_point_to_snapshot(
         self,
         *,
         recoveryPointId: str,
         snapshotName: str,
         retentionPeriod: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ConvertRecoveryPointToSnapshotResponseTypeDef:
         """
         Converts a recovery point to a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.convert_recovery_point_to_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#convert_recovery_point_to_snapshot)
         """
@@ -186,15 +186,15 @@
     async def create_endpoint_access(
         self,
         *,
         endpointName: str,
         subnetIds: Sequence[str],
         workgroupName: str,
         ownerAccount: str = ...,
-        vpcSecurityGroupIds: Sequence[str] = ...
+        vpcSecurityGroupIds: Sequence[str] = ...,
     ) -> CreateEndpointAccessResponseTypeDef:
         """
         Creates an Amazon Redshift Serverless managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_endpoint_access)
         """
@@ -209,15 +209,15 @@
         dbName: str = ...,
         defaultIamRoleArn: str = ...,
         iamRoles: Sequence[str] = ...,
         kmsKeyId: str = ...,
         logExports: Sequence[LogExportType] = ...,
         manageAdminPassword: bool = ...,
         redshiftIdcApplicationArn: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNamespaceResponseTypeDef:
         """
         Creates a namespace in Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_namespace)
         """
@@ -229,45 +229,45 @@
         roleArn: str,
         schedule: ScheduleTypeDef,
         scheduledActionName: str,
         targetAction: TargetActionTypeDef,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         scheduledActionDescription: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> CreateScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_scheduled_action)
         """
 
     async def create_snapshot(
         self,
         *,
         namespaceName: str,
         snapshotName: str,
         retentionPeriod: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a snapshot of all databases in a namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_snapshot)
         """
 
     async def create_snapshot_copy_configuration(
         self,
         *,
         destinationRegion: str,
         namespaceName: str,
         destinationKmsKeyId: str = ...,
-        snapshotRetentionPeriod: int = ...
+        snapshotRetentionPeriod: int = ...,
     ) -> CreateSnapshotCopyConfigurationResponseTypeDef:
         """
         Creates a snapshot copy configuration that lets you copy snapshots to another
         Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_snapshot_copy_configuration)
@@ -277,15 +277,15 @@
     async def create_usage_limit(
         self,
         *,
         amount: int,
         resourceArn: str,
         usageType: UsageLimitUsageTypeType,
         breachAction: UsageLimitBreachActionType = ...,
-        period: UsageLimitPeriodType = ...
+        period: UsageLimitPeriodType = ...,
     ) -> CreateUsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift Serverless usage type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_usage_limit)
         """
@@ -299,15 +299,15 @@
         configParameters: Sequence[ConfigParameterTypeDef] = ...,
         enhancedVpcRouting: bool = ...,
         maxCapacity: int = ...,
         port: int = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkgroupResponseTypeDef:
         """
         Creates an workgroup in Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.create_workgroup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#create_workgroup)
         """
@@ -333,15 +333,15 @@
         """
 
     async def delete_namespace(
         self,
         *,
         namespaceName: str,
         finalSnapshotName: str = ...,
-        finalSnapshotRetentionPeriod: int = ...
+        finalSnapshotRetentionPeriod: int = ...,
     ) -> DeleteNamespaceResponseTypeDef:
         """
         Deletes a namespace from Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.delete_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#delete_namespace)
         """
@@ -415,15 +415,15 @@
 
     async def get_credentials(
         self,
         *,
         customDomainName: str = ...,
         dbName: str = ...,
         durationSeconds: int = ...,
-        workgroupName: str = ...
+        workgroupName: str = ...,
     ) -> GetCredentialsResponseTypeDef:
         """
         Returns a database user name and temporary password with temporary
         authorization to log in to Amazon Redshift
         Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.get_credentials)
@@ -520,15 +520,15 @@
 
     async def list_custom_domain_associations(
         self,
         *,
         customDomainCertificateArn: str = ...,
         customDomainName: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCustomDomainAssociationsResponseTypeDef:
         """
         Lists custom domain associations for Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_custom_domain_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_custom_domain_associations)
         """
@@ -536,15 +536,15 @@
     async def list_endpoint_access(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
         vpcId: str = ...,
-        workgroupName: str = ...
+        workgroupName: str = ...,
     ) -> ListEndpointAccessResponseTypeDef:
         """
         Returns an array of `EndpointAccess` objects and relevant information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_endpoint_access)
         """
@@ -563,15 +563,15 @@
         self,
         *,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListRecoveryPointsResponseTypeDef:
         """
         Returns an array of recovery points.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_recovery_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_recovery_points)
         """
@@ -601,30 +601,30 @@
         *,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListSnapshotsResponseTypeDef:
         """
         Returns a list of snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_snapshots)
         """
 
     async def list_table_restore_status(
         self,
         *,
         maxResults: int = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        workgroupName: str = ...
+        workgroupName: str = ...,
     ) -> ListTableRestoreStatusResponseTypeDef:
         """
         Returns information about an array of `TableRestoreStatus` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_table_restore_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_table_restore_status)
         """
@@ -641,15 +641,15 @@
 
     async def list_usage_limits(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         resourceArn: str = ...,
-        usageType: UsageLimitUsageTypeType = ...
+        usageType: UsageLimitUsageTypeType = ...,
     ) -> ListUsageLimitsResponseTypeDef:
         """
         Lists all usage limits within Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_usage_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#list_usage_limits)
         """
@@ -689,15 +689,15 @@
         *,
         namespaceName: str,
         workgroupName: str,
         adminPasswordSecretKmsKeyId: str = ...,
         manageAdminPassword: bool = ...,
         ownerAccount: str = ...,
         snapshotArn: str = ...,
-        snapshotName: str = ...
+        snapshotName: str = ...,
     ) -> RestoreFromSnapshotResponseTypeDef:
         """
         Restores a namespace from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.restore_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#restore_from_snapshot)
         """
@@ -710,15 +710,15 @@
         recoveryPointId: str,
         sourceDatabaseName: str,
         sourceTableName: str,
         workgroupName: str,
         activateCaseSensitiveIdentifier: bool = ...,
         sourceSchemaName: str = ...,
         targetDatabaseName: str = ...,
-        targetSchemaName: str = ...
+        targetSchemaName: str = ...,
     ) -> RestoreTableFromRecoveryPointResponseTypeDef:
         """
         Restores a table from a recovery point to your Amazon Redshift Serverless
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.restore_table_from_recovery_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#restore_table_from_recovery_point)
@@ -732,15 +732,15 @@
         snapshotName: str,
         sourceDatabaseName: str,
         sourceTableName: str,
         workgroupName: str,
         activateCaseSensitiveIdentifier: bool = ...,
         sourceSchemaName: str = ...,
         targetDatabaseName: str = ...,
-        targetSchemaName: str = ...
+        targetSchemaName: str = ...,
     ) -> RestoreTableFromSnapshotResponseTypeDef:
         """
         Restores a table from a snapshot to your Amazon Redshift Serverless instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.restore_table_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#restore_table_from_snapshot)
         """
@@ -789,15 +789,15 @@
         adminPasswordSecretKmsKeyId: str = ...,
         adminUserPassword: str = ...,
         adminUsername: str = ...,
         defaultIamRoleArn: str = ...,
         iamRoles: Sequence[str] = ...,
         kmsKeyId: str = ...,
         logExports: Sequence[LogExportType] = ...,
-        manageAdminPassword: bool = ...
+        manageAdminPassword: bool = ...,
     ) -> UpdateNamespaceResponseTypeDef:
         """
         Updates a namespace with the specified settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_namespace)
         """
@@ -808,15 +808,15 @@
         scheduledActionName: str,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         roleArn: str = ...,
         schedule: ScheduleTypeDef = ...,
         scheduledActionDescription: str = ...,
         startTime: TimestampTypeDef = ...,
-        targetAction: TargetActionTypeDef = ...
+        targetAction: TargetActionTypeDef = ...,
     ) -> UpdateScheduledActionResponseTypeDef:
         """
         Updates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_scheduled_action)
         """
@@ -842,15 +842,15 @@
         """
 
     async def update_usage_limit(
         self,
         *,
         usageLimitId: str,
         amount: int = ...,
-        breachAction: UsageLimitBreachActionType = ...
+        breachAction: UsageLimitBreachActionType = ...,
     ) -> UpdateUsageLimitResponseTypeDef:
         """
         Update a usage limit in Amazon Redshift Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_usage_limit)
         """
@@ -862,15 +862,15 @@
         baseCapacity: int = ...,
         configParameters: Sequence[ConfigParameterTypeDef] = ...,
         enhancedVpcRouting: bool = ...,
         maxCapacity: int = ...,
         port: int = ...,
         publiclyAccessible: bool = ...,
         securityGroupIds: Sequence[str] = ...,
-        subnetIds: Sequence[str] = ...
+        subnetIds: Sequence[str] = ...,
     ) -> UpdateWorkgroupResponseTypeDef:
         """
         Updates a workgroup with the specified configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_workgroup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/client/#update_workgroup)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/literals.py` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/literals.py`

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
     "ListCustomDomainAssociationsPaginatorName",
     "ListEndpointAccessPaginatorName",
     "ListNamespacesPaginatorName",
     "ListRecoveryPointsPaginatorName",
     "ListScheduledActionsPaginatorName",
     "ListSnapshotCopyConfigurationsPaginatorName",
@@ -42,15 +41,14 @@
     "RedshiftServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListCustomDomainAssociationsPaginatorName = Literal["list_custom_domain_associations"]
 ListEndpointAccessPaginatorName = Literal["list_endpoint_access"]
 ListNamespacesPaginatorName = Literal["list_namespaces"]
 ListRecoveryPointsPaginatorName = Literal["list_recovery_points"]
 ListScheduledActionsPaginatorName = Literal["list_scheduled_actions"]
 ListSnapshotCopyConfigurationsPaginatorName = Literal["list_snapshot_copy_configurations"]
 ListSnapshotsPaginatorName = Literal["list_snapshots"]
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/literals.pyi` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/paginator.py` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     "ListSnapshotCopyConfigurationsPaginator",
     "ListSnapshotsPaginator",
     "ListTableRestoreStatusPaginator",
     "ListUsageLimitsPaginator",
     "ListWorkgroupsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -91,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         customDomainCertificateArn: str = ...,
         customDomainName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomDomainAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListCustomDomainAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listcustomdomainassociationspaginator)
         """
 
 
@@ -111,15 +110,15 @@
 
     def paginate(
         self,
         *,
         ownerAccount: str = ...,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
 
@@ -147,15 +146,15 @@
     def paginate(
         self,
         *,
         endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         startTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
 
@@ -199,15 +198,15 @@
         self,
         *,
         endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
         startTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
 
@@ -218,15 +217,15 @@
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
 
@@ -237,15 +236,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listusagelimitspaginator)
         """
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/paginator.pyi` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         customDomainCertificateArn: str = ...,
         customDomainName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomDomainAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListCustomDomainAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listcustomdomainassociationspaginator)
         """
 
 class ListEndpointAccessPaginator(AioPaginator):
@@ -107,15 +107,15 @@
 
     def paginate(
         self,
         *,
         ownerAccount: str = ...,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
 class ListNamespacesPaginator(AioPaginator):
@@ -141,15 +141,15 @@
     def paginate(
         self,
         *,
         endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         startTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
 class ListScheduledActionsPaginator(AioPaginator):
@@ -190,15 +190,15 @@
         self,
         *,
         endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
         startTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
 class ListTableRestoreStatusPaginator(AioPaginator):
@@ -208,15 +208,15 @@
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
 class ListUsageLimitsPaginator(AioPaginator):
@@ -226,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
 class ListWorkgroupsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/type_defs.py` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociationTypeDef",
     "ConfigParameterTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateCustomDomainAssociationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless/type_defs.pyi` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-serverless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RedshiftServerless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RedshiftServerless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/
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
 
 <a id="types-aiobotocore-redshift-serverless"></a>
 
 # types-aiobotocore-redshift-serverless
 
 [![PyPI - types-aiobotocore-redshift-serverless](https://img.shields.io/pypi/v/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[aiobotocore.RedshiftServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [types-aiobotocore-redshift-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-redshift-serverless-2.9.0/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-serverless-2.9.1/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

