# Comparing `tmp/types-aiobotocore-servicecatalog-2.9.0.tar.gz` & `tmp/types-aiobotocore-servicecatalog-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicecatalog-2.9.0.tar", last modified: Wed Dec 13 20:00:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicecatalog-2.9.1.tar", last modified: Thu Jan 18 01:21:48 2024, max compression
```

## Comparing `types-aiobotocore-servicecatalog-2.9.0.tar` & `types-aiobotocore-servicecatalog-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:30.233140 types-aiobotocore-servicecatalog-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2023-12-13 20:00:30.233140 types-aiobotocore-servicecatalog-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:30.233140 types-aiobotocore-servicecatalog-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:30.233140 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79861 2023-12-13 19:56:18.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    79857 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15483 2023-12-13 19:56:18.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15481 2023-12-13 19:56:18.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22689 2023-12-13 19:56:18.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22670 2023-12-13 19:56:18.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    80829 2023-12-13 19:56:23.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80828 2023-12-13 19:56:19.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:17.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:30.233140 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2023-12-13 20:00:30.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:30.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:30.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:30.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:30.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:30.000000 types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.673035 types-aiobotocore-servicecatalog-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-01-18 01:21:48.673035 types-aiobotocore-servicecatalog-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:48.673035 types-aiobotocore-servicecatalog-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.673035 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79916 2024-01-18 01:17:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79913 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15481 2024-01-18 01:17:52.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15481 2024-01-18 01:17:52.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-01-18 01:17:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-01-18 01:17:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    80828 2024-01-18 01:17:54.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80828 2024-01-18 01:17:53.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:47.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.673035 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:48.000000 types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/LICENSE` & `types-aiobotocore-servicecatalog-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-servicecatalog-2.9.0/PKG-INFO` & `types-aiobotocore-servicecatalog-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServiceCatalog 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServiceCatalog 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/
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
 
 <a id="types-aiobotocore-servicecatalog"></a>
 
 # types-aiobotocore-servicecatalog
 
 [![PyPI - types-aiobotocore-servicecatalog](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog)](https://pepy.tech/project/types-aiobotocore-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceCatalog 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[aiobotocore.ServiceCatalog 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [types-aiobotocore-servicecatalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/README.md` & `types-aiobotocore-servicecatalog-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog)](https://pepy.tech/project/types-aiobotocore-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceCatalog 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[aiobotocore.ServiceCatalog 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [types-aiobotocore-servicecatalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/setup.py` & `types-aiobotocore-servicecatalog-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicecatalog",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServiceCatalog 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ServiceCatalog 2.9.1 service generated with"
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
     keywords="aiobotocore servicecatalog type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_servicecatalog": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/__init__.py` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ListTagOptionsPaginator,
     ScanProvisionedProductsPaginator,
     SearchProductsAsAdminPaginator,
 )
 
 Client = ServiceCatalogClient
 
-
 __all__ = (
     "Client",
     "ListAcceptedPortfolioSharesPaginator",
     "ListConstraintsForPortfolioPaginator",
     "ListLaunchPathsPaginator",
     "ListOrganizationPortfolioAccessPaginator",
     "ListPortfoliosForProductPaginator",
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/__init__.pyi` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/__main__.py` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceCatalog 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ServiceCatalog 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
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

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/client.py` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ServiceCatalogClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -183,15 +182,15 @@
         """
 
     async def accept_portfolio_share(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PortfolioShareType: PortfolioShareTypeType = ...
+        PortfolioShareType: PortfolioShareTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Accepts an offer to share the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.accept_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#accept_portfolio_share)
         """
@@ -208,45 +207,45 @@
 
     async def associate_principal_with_portfolio(
         self,
         *,
         PortfolioId: str,
         PrincipalARN: str,
         PrincipalType: PrincipalTypeType,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> Dict[str, Any]:
         """
         Associates the specified principal ARN with the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.associate_principal_with_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_principal_with_portfolio)
         """
 
     async def associate_product_with_portfolio(
         self,
         *,
         ProductId: str,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        SourcePortfolioId: str = ...
+        SourcePortfolioId: str = ...,
     ) -> Dict[str, Any]:
         """
         Associates the specified product with the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.associate_product_with_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_product_with_portfolio)
         """
 
     async def associate_service_action_with_provisioning_artifact(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         ServiceActionId: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> Dict[str, Any]:
         """
         Associates a self-service action with a provisioning artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.associate_service_action_with_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_service_action_with_provisioning_artifact)
         """
@@ -261,28 +260,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_tag_option_with_resource)
         """
 
     async def batch_associate_service_action_with_provisioning_artifact(
         self,
         *,
         ServiceActionAssociations: Sequence[ServiceActionAssociationTypeDef],
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef:
         """
         Associates multiple self-service actions with provisioning artifacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.batch_associate_service_action_with_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#batch_associate_service_action_with_provisioning_artifact)
         """
 
     async def batch_disassociate_service_action_from_provisioning_artifact(
         self,
         *,
         ServiceActionAssociations: Sequence[ServiceActionAssociationTypeDef],
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef:
         """
         Disassociates a batch of self-service actions from the specified provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.batch_disassociate_service_action_from_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#batch_disassociate_service_action_from_provisioning_artifact)
@@ -309,15 +308,15 @@
         *,
         SourceProductArn: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
         TargetProductId: str = ...,
         TargetProductName: str = ...,
         SourceProvisioningArtifactIdentifiers: Sequence[Mapping[Literal["Id"], str]] = ...,
-        CopyOptions: Sequence[Literal["CopyTags"]] = ...
+        CopyOptions: Sequence[Literal["CopyTags"]] = ...,
     ) -> CopyProductOutputTypeDef:
         """
         Copies the specified source product to the specified target product or a new
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.copy_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#copy_product)
@@ -328,15 +327,15 @@
         *,
         PortfolioId: str,
         ProductId: str,
         Parameters: str,
         Type: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateConstraintOutputTypeDef:
         """
         Creates a constraint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_constraint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_constraint)
         """
@@ -345,15 +344,15 @@
         self,
         *,
         DisplayName: str,
         ProviderName: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePortfolioOutputTypeDef:
         """
         Creates a portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_portfolio)
         """
@@ -362,15 +361,15 @@
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         AccountId: str = ...,
         OrganizationNode: OrganizationNodeTypeDef = ...,
         ShareTagOptions: bool = ...,
-        SharePrincipals: bool = ...
+        SharePrincipals: bool = ...,
     ) -> CreatePortfolioShareOutputTypeDef:
         """
         Shares the specified portfolio with the specified account or organization node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_portfolio_share)
         """
@@ -386,15 +385,15 @@
         Description: str = ...,
         Distributor: str = ...,
         SupportDescription: str = ...,
         SupportEmail: str = ...,
         SupportUrl: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ProvisioningArtifactParameters: ProvisioningArtifactPropertiesTypeDef = ...,
-        SourceConnection: SourceConnectionTypeDef = ...
+        SourceConnection: SourceConnectionTypeDef = ...,
     ) -> CreateProductOutputTypeDef:
         """
         Creates a product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_product)
         """
@@ -408,30 +407,30 @@
         ProvisionedProductName: str,
         ProvisioningArtifactId: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
         NotificationArns: Sequence[str] = ...,
         PathId: str = ...,
         ProvisioningParameters: Sequence[UpdateProvisioningParameterTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProvisionedProductPlanOutputTypeDef:
         """
         Creates a plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_provisioned_product_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_provisioned_product_plan)
         """
 
     async def create_provisioning_artifact(
         self,
         *,
         ProductId: str,
         Parameters: ProvisioningArtifactPropertiesTypeDef,
         IdempotencyToken: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> CreateProvisioningArtifactOutputTypeDef:
         """
         Creates a provisioning artifact (also known as a version) for the specified
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_provisioning_artifact)
@@ -441,15 +440,15 @@
         self,
         *,
         Name: str,
         DefinitionType: Literal["SSM_AUTOMATION"],
         Definition: Mapping[ServiceActionDefinitionKeyType, str],
         IdempotencyToken: str,
         Description: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> CreateServiceActionOutputTypeDef:
         """
         Creates a self-service action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_service_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_service_action)
         """
@@ -480,15 +479,15 @@
 
     async def delete_portfolio_share(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         AccountId: str = ...,
-        OrganizationNode: OrganizationNodeTypeDef = ...
+        OrganizationNode: OrganizationNodeTypeDef = ...,
     ) -> DeletePortfolioShareOutputTypeDef:
         """
         Stops sharing the specified portfolio with the specified account or
         organization
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.delete_portfolio_share)
@@ -583,15 +582,15 @@
 
     async def describe_portfolio_shares(
         self,
         *,
         PortfolioId: str,
         Type: DescribePortfolioShareTypeType,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribePortfolioSharesOutputTypeDef:
         """
         Returns a summary of each of the portfolio shares that were created for the
         specified
         portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_portfolio_shares)
@@ -610,15 +609,15 @@
 
     async def describe_product_as_admin(
         self,
         *,
         AcceptLanguage: str = ...,
         Id: str = ...,
         Name: str = ...,
-        SourcePortfolioId: str = ...
+        SourcePortfolioId: str = ...,
     ) -> DescribeProductAsAdminOutputTypeDef:
         """
         Gets information about the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_product_as_admin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#describe_product_as_admin)
         """
@@ -658,15 +657,15 @@
         *,
         AcceptLanguage: str = ...,
         ProvisioningArtifactId: str = ...,
         ProductId: str = ...,
         ProvisioningArtifactName: str = ...,
         ProductName: str = ...,
         Verbose: bool = ...,
-        IncludeProvisioningArtifactParameters: bool = ...
+        IncludeProvisioningArtifactParameters: bool = ...,
     ) -> DescribeProvisioningArtifactOutputTypeDef:
         """
         Gets information about the specified provisioning artifact (also known as a
         version) for the specified
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_provisioning_artifact)
@@ -678,15 +677,15 @@
         *,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
         ProductName: str = ...,
         ProvisioningArtifactId: str = ...,
         ProvisioningArtifactName: str = ...,
         PathId: str = ...,
-        PathName: str = ...
+        PathName: str = ...,
     ) -> DescribeProvisioningParametersOutputTypeDef:
         """
         Gets information about the configuration required to provision the specified
         product using the specified provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_provisioning_parameters)
@@ -753,15 +752,15 @@
 
     async def disassociate_principal_from_portfolio(
         self,
         *,
         PortfolioId: str,
         PrincipalARN: str,
         AcceptLanguage: str = ...,
-        PrincipalType: PrincipalTypeType = ...
+        PrincipalType: PrincipalTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Disassociates a previously associated principal ARN from a specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.disassociate_principal_from_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#disassociate_principal_from_portfolio)
         """
@@ -778,15 +777,15 @@
 
     async def disassociate_service_action_from_provisioning_artifact(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         ServiceActionId: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> Dict[str, Any]:
         """
         Disassociates the specified self-service action association from the specified
         provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.disassociate_service_action_from_provisioning_artifact)
@@ -826,15 +825,15 @@
     async def execute_provisioned_product_service_action(
         self,
         *,
         ProvisionedProductId: str,
         ServiceActionId: str,
         ExecuteToken: str,
         AcceptLanguage: str = ...,
-        Parameters: Mapping[str, Sequence[str]] = ...
+        Parameters: Mapping[str, Sequence[str]] = ...,
     ) -> ExecuteProvisionedProductServiceActionOutputTypeDef:
         """
         Executes a self-service action against a provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.execute_provisioned_product_service_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#execute_provisioned_product_service_action)
         """
@@ -867,15 +866,15 @@
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionedProductId: str = ...,
         ProvisionedProductName: str = ...,
         OutputKeys: Sequence[str] = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> GetProvisionedProductOutputsOutputTypeDef:
         """
         This API takes either a `ProvisonedProductId` or a `ProvisionedProductName`,
         along with a list of one or more output keys, and responds with the key/value
         pairs of those
         outputs.
 
@@ -887,15 +886,15 @@
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         ProvisionedProductName: str,
         PhysicalId: str,
         IdempotencyToken: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> ImportAsProvisionedProductOutputTypeDef:
         """
         Requests the import of a resource as an Service Catalog provisioned product
         that is associated to an Service Catalog product and provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.import_as_provisioned_product)
@@ -904,15 +903,15 @@
 
     async def list_accepted_portfolio_shares(
         self,
         *,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
         PageSize: int = ...,
-        PortfolioShareType: PortfolioShareTypeType = ...
+        PortfolioShareType: PortfolioShareTypeType = ...,
     ) -> ListAcceptedPortfolioSharesOutputTypeDef:
         """
         Lists all imported portfolios for which account-to-account shares were accepted
         by this
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_accepted_portfolio_shares)
@@ -921,15 +920,15 @@
 
     async def list_budgets_for_resource(
         self,
         *,
         ResourceId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListBudgetsForResourceOutputTypeDef:
         """
         Lists all the budgets associated to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_budgets_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_budgets_for_resource)
         """
@@ -937,30 +936,30 @@
     async def list_constraints_for_portfolio(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListConstraintsForPortfolioOutputTypeDef:
         """
         Lists the constraints for the specified portfolio and product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_constraints_for_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_constraints_for_portfolio)
         """
 
     async def list_launch_paths(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListLaunchPathsOutputTypeDef:
         """
         Lists the paths to the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_launch_paths)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_launch_paths)
         """
@@ -968,15 +967,15 @@
     async def list_organization_portfolio_access(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListOrganizationPortfolioAccessOutputTypeDef:
         """
         Lists the organization nodes that have access to the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_organization_portfolio_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_organization_portfolio_access)
         """
@@ -984,15 +983,15 @@
     async def list_portfolio_access(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         OrganizationParentId: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListPortfolioAccessOutputTypeDef:
         """
         Lists the account IDs that have access to the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_portfolio_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_portfolio_access)
         """
@@ -1009,30 +1008,30 @@
 
     async def list_portfolios_for_product(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListPortfoliosForProductOutputTypeDef:
         """
         Lists all portfolios that the specified product is associated with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_portfolios_for_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_portfolios_for_product)
         """
 
     async def list_principals_for_portfolio(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListPrincipalsForPortfolioOutputTypeDef:
         """
         Lists all `PrincipalARN`s and corresponding `PrincipalType`s associated with
         the specified
         portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_principals_for_portfolio)
@@ -1042,15 +1041,15 @@
     async def list_provisioned_product_plans(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         PageSize: int = ...,
         PageToken: str = ...,
-        AccessLevelFilter: AccessLevelFilterTypeDef = ...
+        AccessLevelFilter: AccessLevelFilterTypeDef = ...,
     ) -> ListProvisionedProductPlansOutputTypeDef:
         """
         Lists the plans for the specified provisioned product or all plans to which the
         user has
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_provisioned_product_plans)
@@ -1070,15 +1069,15 @@
 
     async def list_provisioning_artifacts_for_service_action(
         self,
         *,
         ServiceActionId: str,
         PageSize: int = ...,
         PageToken: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> ListProvisioningArtifactsForServiceActionOutputTypeDef:
         """
         Lists all provisioning artifacts (also known as versions) for the specified
         self-service
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_provisioning_artifacts_for_service_action)
@@ -1088,30 +1087,30 @@
     async def list_record_history(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListRecordHistoryOutputTypeDef:
         """
         Lists the specified requests or all performed requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_record_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_record_history)
         """
 
     async def list_resources_for_tag_option(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListResourcesForTagOptionOutputTypeDef:
         """
         Lists the resources associated with the specified TagOption.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_resources_for_tag_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_resources_for_tag_option)
         """
@@ -1129,15 +1128,15 @@
     async def list_service_actions_for_provisioning_artifact(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         PageSize: int = ...,
         PageToken: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> ListServiceActionsForProvisioningArtifactOutputTypeDef:
         """
         Returns a paginated list of self-service actions associated with the specified
         Product ID and Provisioning Artifact
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_service_actions_for_provisioning_artifact)
@@ -1146,15 +1145,15 @@
 
     async def list_stack_instances_for_provisioned_product(
         self,
         *,
         ProvisionedProductId: str,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListStackInstancesForProvisionedProductOutputTypeDef:
         """
         Returns summary information about stack instances that are associated with the
         specified `CFN_STACKSET` type provisioned
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_stack_instances_for_provisioned_product)
@@ -1162,15 +1161,15 @@
         """
 
     async def list_tag_options(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListTagOptionsOutputTypeDef:
         """
         Lists the specified TagOptions or all TagOptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_tag_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_tag_options)
         """
@@ -1180,15 +1179,15 @@
         *,
         WorkflowToken: str,
         RecordId: str,
         Status: EngineWorkflowStatusType,
         IdempotencyToken: str,
         FailureReason: str = ...,
         ResourceIdentifier: EngineWorkflowResourceIdentifierTypeDef = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
+        Outputs: Sequence[RecordOutputTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Notifies the result of the provisioning engine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_provision_product_engine_workflow_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#notify_provision_product_engine_workflow_result)
         """
@@ -1196,15 +1195,15 @@
     async def notify_terminate_provisioned_product_engine_workflow_result(
         self,
         *,
         WorkflowToken: str,
         RecordId: str,
         Status: EngineWorkflowStatusType,
         IdempotencyToken: str,
-        FailureReason: str = ...
+        FailureReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Notifies the result of the terminate engine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_terminate_provisioned_product_engine_workflow_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#notify_terminate_provisioned_product_engine_workflow_result)
         """
@@ -1213,15 +1212,15 @@
         self,
         *,
         WorkflowToken: str,
         RecordId: str,
         Status: EngineWorkflowStatusType,
         IdempotencyToken: str,
         FailureReason: str = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
+        Outputs: Sequence[RecordOutputTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Notifies the result of the update engine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_update_provisioned_product_engine_workflow_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#notify_update_provisioned_product_engine_workflow_result)
         """
@@ -1237,44 +1236,44 @@
         ProvisioningArtifactId: str = ...,
         ProvisioningArtifactName: str = ...,
         PathId: str = ...,
         PathName: str = ...,
         ProvisioningParameters: Sequence[ProvisioningParameterTypeDef] = ...,
         ProvisioningPreferences: ProvisioningPreferencesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        NotificationArns: Sequence[str] = ...
+        NotificationArns: Sequence[str] = ...,
     ) -> ProvisionProductOutputTypeDef:
         """
         Provisions the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.provision_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#provision_product)
         """
 
     async def reject_portfolio_share(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PortfolioShareType: PortfolioShareTypeType = ...
+        PortfolioShareType: PortfolioShareTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Rejects an offer to share the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.reject_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#reject_portfolio_share)
         """
 
     async def scan_provisioned_products(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ScanProvisionedProductsOutputTypeDef:
         """
         Lists the provisioned products that are available (not terminated).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.scan_provisioned_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#scan_provisioned_products)
         """
@@ -1283,15 +1282,15 @@
         self,
         *,
         AcceptLanguage: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         PageSize: int = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> SearchProductsOutputTypeDef:
         """
         Gets information about the products to which the caller has access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.search_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#search_products)
         """
@@ -1302,15 +1301,15 @@
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         PageToken: str = ...,
         PageSize: int = ...,
-        ProductSource: Literal["ACCOUNT"] = ...
+        ProductSource: Literal["ACCOUNT"] = ...,
     ) -> SearchProductsAsAdminOutputTypeDef:
         """
         Gets information about the products for the specified portfolio or all products.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.search_products_as_admin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#search_products_as_admin)
         """
@@ -1320,15 +1319,15 @@
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         Filters: Mapping[Literal["SearchQuery"], Sequence[str]] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> SearchProvisionedProductsOutputTypeDef:
         """
         Gets information about the provisioned products that meet the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.search_provisioned_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#search_provisioned_products)
@@ -1338,15 +1337,15 @@
         self,
         *,
         TerminateToken: str,
         ProvisionedProductName: str = ...,
         ProvisionedProductId: str = ...,
         IgnoreErrors: bool = ...,
         AcceptLanguage: str = ...,
-        RetainPhysicalResources: bool = ...
+        RetainPhysicalResources: bool = ...,
     ) -> TerminateProvisionedProductOutputTypeDef:
         """
         Terminates the specified provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.terminate_provisioned_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#terminate_provisioned_product)
         """
@@ -1366,15 +1365,15 @@
         *,
         Id: str,
         AcceptLanguage: str = ...,
         DisplayName: str = ...,
         Description: str = ...,
         ProviderName: str = ...,
         AddTags: Sequence[TagTypeDef] = ...,
-        RemoveTags: Sequence[str] = ...
+        RemoveTags: Sequence[str] = ...,
     ) -> UpdatePortfolioOutputTypeDef:
         """
         Updates the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_portfolio)
         """
@@ -1383,15 +1382,15 @@
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         AccountId: str = ...,
         OrganizationNode: OrganizationNodeTypeDef = ...,
         ShareTagOptions: bool = ...,
-        SharePrincipals: bool = ...
+        SharePrincipals: bool = ...,
     ) -> UpdatePortfolioShareOutputTypeDef:
         """
         Updates the specified portfolio share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_portfolio_share)
         """
@@ -1406,15 +1405,15 @@
         Description: str = ...,
         Distributor: str = ...,
         SupportDescription: str = ...,
         SupportEmail: str = ...,
         SupportUrl: str = ...,
         AddTags: Sequence[TagTypeDef] = ...,
         RemoveTags: Sequence[str] = ...,
-        SourceConnection: SourceConnectionTypeDef = ...
+        SourceConnection: SourceConnectionTypeDef = ...,
     ) -> UpdateProductOutputTypeDef:
         """
         Updates the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_product)
         """
@@ -1430,30 +1429,30 @@
         ProductName: str = ...,
         ProvisioningArtifactId: str = ...,
         ProvisioningArtifactName: str = ...,
         PathId: str = ...,
         PathName: str = ...,
         ProvisioningParameters: Sequence[UpdateProvisioningParameterTypeDef] = ...,
         ProvisioningPreferences: UpdateProvisioningPreferencesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateProvisionedProductOutputTypeDef:
         """
         Requests updates to the configuration of the specified provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_provisioned_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_provisioned_product)
         """
 
     async def update_provisioned_product_properties(
         self,
         *,
         ProvisionedProductId: str,
         ProvisionedProductProperties: Mapping[PropertyKeyType, str],
         IdempotencyToken: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> UpdateProvisionedProductPropertiesOutputTypeDef:
         """
         Requests updates to the properties of the specified provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_provisioned_product_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_provisioned_product_properties)
         """
@@ -1463,15 +1462,15 @@
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
         Name: str = ...,
         Description: str = ...,
         Active: bool = ...,
-        Guidance: ProvisioningArtifactGuidanceType = ...
+        Guidance: ProvisioningArtifactGuidanceType = ...,
     ) -> UpdateProvisioningArtifactOutputTypeDef:
         """
         Updates the specified provisioning artifact (also known as a version) for the
         specified
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_provisioning_artifact)
@@ -1481,15 +1480,15 @@
     async def update_service_action(
         self,
         *,
         Id: str,
         Name: str = ...,
         Definition: Mapping[ServiceActionDefinitionKeyType, str] = ...,
         Description: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> UpdateServiceActionOutputTypeDef:
         """
         Updates a self-service action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_service_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_service_action)
         """
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/client.pyi` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         """
 
     async def accept_portfolio_share(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PortfolioShareType: PortfolioShareTypeType = ...
+        PortfolioShareType: PortfolioShareTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Accepts an offer to share the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.accept_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#accept_portfolio_share)
         """
@@ -204,45 +204,45 @@
 
     async def associate_principal_with_portfolio(
         self,
         *,
         PortfolioId: str,
         PrincipalARN: str,
         PrincipalType: PrincipalTypeType,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> Dict[str, Any]:
         """
         Associates the specified principal ARN with the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.associate_principal_with_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_principal_with_portfolio)
         """
 
     async def associate_product_with_portfolio(
         self,
         *,
         ProductId: str,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        SourcePortfolioId: str = ...
+        SourcePortfolioId: str = ...,
     ) -> Dict[str, Any]:
         """
         Associates the specified product with the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.associate_product_with_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_product_with_portfolio)
         """
 
     async def associate_service_action_with_provisioning_artifact(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         ServiceActionId: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> Dict[str, Any]:
         """
         Associates a self-service action with a provisioning artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.associate_service_action_with_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_service_action_with_provisioning_artifact)
         """
@@ -257,28 +257,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#associate_tag_option_with_resource)
         """
 
     async def batch_associate_service_action_with_provisioning_artifact(
         self,
         *,
         ServiceActionAssociations: Sequence[ServiceActionAssociationTypeDef],
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef:
         """
         Associates multiple self-service actions with provisioning artifacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.batch_associate_service_action_with_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#batch_associate_service_action_with_provisioning_artifact)
         """
 
     async def batch_disassociate_service_action_from_provisioning_artifact(
         self,
         *,
         ServiceActionAssociations: Sequence[ServiceActionAssociationTypeDef],
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef:
         """
         Disassociates a batch of self-service actions from the specified provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.batch_disassociate_service_action_from_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#batch_disassociate_service_action_from_provisioning_artifact)
@@ -305,15 +305,15 @@
         *,
         SourceProductArn: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
         TargetProductId: str = ...,
         TargetProductName: str = ...,
         SourceProvisioningArtifactIdentifiers: Sequence[Mapping[Literal["Id"], str]] = ...,
-        CopyOptions: Sequence[Literal["CopyTags"]] = ...
+        CopyOptions: Sequence[Literal["CopyTags"]] = ...,
     ) -> CopyProductOutputTypeDef:
         """
         Copies the specified source product to the specified target product or a new
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.copy_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#copy_product)
@@ -324,15 +324,15 @@
         *,
         PortfolioId: str,
         ProductId: str,
         Parameters: str,
         Type: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateConstraintOutputTypeDef:
         """
         Creates a constraint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_constraint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_constraint)
         """
@@ -341,15 +341,15 @@
         self,
         *,
         DisplayName: str,
         ProviderName: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePortfolioOutputTypeDef:
         """
         Creates a portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_portfolio)
         """
@@ -358,15 +358,15 @@
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         AccountId: str = ...,
         OrganizationNode: OrganizationNodeTypeDef = ...,
         ShareTagOptions: bool = ...,
-        SharePrincipals: bool = ...
+        SharePrincipals: bool = ...,
     ) -> CreatePortfolioShareOutputTypeDef:
         """
         Shares the specified portfolio with the specified account or organization node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_portfolio_share)
         """
@@ -382,15 +382,15 @@
         Description: str = ...,
         Distributor: str = ...,
         SupportDescription: str = ...,
         SupportEmail: str = ...,
         SupportUrl: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ProvisioningArtifactParameters: ProvisioningArtifactPropertiesTypeDef = ...,
-        SourceConnection: SourceConnectionTypeDef = ...
+        SourceConnection: SourceConnectionTypeDef = ...,
     ) -> CreateProductOutputTypeDef:
         """
         Creates a product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_product)
         """
@@ -404,30 +404,30 @@
         ProvisionedProductName: str,
         ProvisioningArtifactId: str,
         IdempotencyToken: str,
         AcceptLanguage: str = ...,
         NotificationArns: Sequence[str] = ...,
         PathId: str = ...,
         ProvisioningParameters: Sequence[UpdateProvisioningParameterTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProvisionedProductPlanOutputTypeDef:
         """
         Creates a plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_provisioned_product_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_provisioned_product_plan)
         """
 
     async def create_provisioning_artifact(
         self,
         *,
         ProductId: str,
         Parameters: ProvisioningArtifactPropertiesTypeDef,
         IdempotencyToken: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> CreateProvisioningArtifactOutputTypeDef:
         """
         Creates a provisioning artifact (also known as a version) for the specified
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_provisioning_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_provisioning_artifact)
@@ -437,15 +437,15 @@
         self,
         *,
         Name: str,
         DefinitionType: Literal["SSM_AUTOMATION"],
         Definition: Mapping[ServiceActionDefinitionKeyType, str],
         IdempotencyToken: str,
         Description: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> CreateServiceActionOutputTypeDef:
         """
         Creates a self-service action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.create_service_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#create_service_action)
         """
@@ -476,15 +476,15 @@
 
     async def delete_portfolio_share(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         AccountId: str = ...,
-        OrganizationNode: OrganizationNodeTypeDef = ...
+        OrganizationNode: OrganizationNodeTypeDef = ...,
     ) -> DeletePortfolioShareOutputTypeDef:
         """
         Stops sharing the specified portfolio with the specified account or
         organization
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.delete_portfolio_share)
@@ -579,15 +579,15 @@
 
     async def describe_portfolio_shares(
         self,
         *,
         PortfolioId: str,
         Type: DescribePortfolioShareTypeType,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribePortfolioSharesOutputTypeDef:
         """
         Returns a summary of each of the portfolio shares that were created for the
         specified
         portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_portfolio_shares)
@@ -606,15 +606,15 @@
 
     async def describe_product_as_admin(
         self,
         *,
         AcceptLanguage: str = ...,
         Id: str = ...,
         Name: str = ...,
-        SourcePortfolioId: str = ...
+        SourcePortfolioId: str = ...,
     ) -> DescribeProductAsAdminOutputTypeDef:
         """
         Gets information about the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_product_as_admin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#describe_product_as_admin)
         """
@@ -654,15 +654,15 @@
         *,
         AcceptLanguage: str = ...,
         ProvisioningArtifactId: str = ...,
         ProductId: str = ...,
         ProvisioningArtifactName: str = ...,
         ProductName: str = ...,
         Verbose: bool = ...,
-        IncludeProvisioningArtifactParameters: bool = ...
+        IncludeProvisioningArtifactParameters: bool = ...,
     ) -> DescribeProvisioningArtifactOutputTypeDef:
         """
         Gets information about the specified provisioning artifact (also known as a
         version) for the specified
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_provisioning_artifact)
@@ -674,15 +674,15 @@
         *,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
         ProductName: str = ...,
         ProvisioningArtifactId: str = ...,
         ProvisioningArtifactName: str = ...,
         PathId: str = ...,
-        PathName: str = ...
+        PathName: str = ...,
     ) -> DescribeProvisioningParametersOutputTypeDef:
         """
         Gets information about the configuration required to provision the specified
         product using the specified provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_provisioning_parameters)
@@ -749,15 +749,15 @@
 
     async def disassociate_principal_from_portfolio(
         self,
         *,
         PortfolioId: str,
         PrincipalARN: str,
         AcceptLanguage: str = ...,
-        PrincipalType: PrincipalTypeType = ...
+        PrincipalType: PrincipalTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Disassociates a previously associated principal ARN from a specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.disassociate_principal_from_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#disassociate_principal_from_portfolio)
         """
@@ -774,15 +774,15 @@
 
     async def disassociate_service_action_from_provisioning_artifact(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         ServiceActionId: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> Dict[str, Any]:
         """
         Disassociates the specified self-service action association from the specified
         provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.disassociate_service_action_from_provisioning_artifact)
@@ -822,15 +822,15 @@
     async def execute_provisioned_product_service_action(
         self,
         *,
         ProvisionedProductId: str,
         ServiceActionId: str,
         ExecuteToken: str,
         AcceptLanguage: str = ...,
-        Parameters: Mapping[str, Sequence[str]] = ...
+        Parameters: Mapping[str, Sequence[str]] = ...,
     ) -> ExecuteProvisionedProductServiceActionOutputTypeDef:
         """
         Executes a self-service action against a provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.execute_provisioned_product_service_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#execute_provisioned_product_service_action)
         """
@@ -863,15 +863,15 @@
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionedProductId: str = ...,
         ProvisionedProductName: str = ...,
         OutputKeys: Sequence[str] = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> GetProvisionedProductOutputsOutputTypeDef:
         """
         This API takes either a `ProvisonedProductId` or a `ProvisionedProductName`,
         along with a list of one or more output keys, and responds with the key/value
         pairs of those
         outputs.
 
@@ -883,15 +883,15 @@
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         ProvisionedProductName: str,
         PhysicalId: str,
         IdempotencyToken: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> ImportAsProvisionedProductOutputTypeDef:
         """
         Requests the import of a resource as an Service Catalog provisioned product
         that is associated to an Service Catalog product and provisioning
         artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.import_as_provisioned_product)
@@ -900,15 +900,15 @@
 
     async def list_accepted_portfolio_shares(
         self,
         *,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
         PageSize: int = ...,
-        PortfolioShareType: PortfolioShareTypeType = ...
+        PortfolioShareType: PortfolioShareTypeType = ...,
     ) -> ListAcceptedPortfolioSharesOutputTypeDef:
         """
         Lists all imported portfolios for which account-to-account shares were accepted
         by this
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_accepted_portfolio_shares)
@@ -917,15 +917,15 @@
 
     async def list_budgets_for_resource(
         self,
         *,
         ResourceId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListBudgetsForResourceOutputTypeDef:
         """
         Lists all the budgets associated to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_budgets_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_budgets_for_resource)
         """
@@ -933,30 +933,30 @@
     async def list_constraints_for_portfolio(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListConstraintsForPortfolioOutputTypeDef:
         """
         Lists the constraints for the specified portfolio and product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_constraints_for_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_constraints_for_portfolio)
         """
 
     async def list_launch_paths(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListLaunchPathsOutputTypeDef:
         """
         Lists the paths to the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_launch_paths)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_launch_paths)
         """
@@ -964,15 +964,15 @@
     async def list_organization_portfolio_access(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListOrganizationPortfolioAccessOutputTypeDef:
         """
         Lists the organization nodes that have access to the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_organization_portfolio_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_organization_portfolio_access)
         """
@@ -980,15 +980,15 @@
     async def list_portfolio_access(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         OrganizationParentId: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListPortfolioAccessOutputTypeDef:
         """
         Lists the account IDs that have access to the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_portfolio_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_portfolio_access)
         """
@@ -1005,30 +1005,30 @@
 
     async def list_portfolios_for_product(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListPortfoliosForProductOutputTypeDef:
         """
         Lists all portfolios that the specified product is associated with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_portfolios_for_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_portfolios_for_product)
         """
 
     async def list_principals_for_portfolio(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListPrincipalsForPortfolioOutputTypeDef:
         """
         Lists all `PrincipalARN`s and corresponding `PrincipalType`s associated with
         the specified
         portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_principals_for_portfolio)
@@ -1038,15 +1038,15 @@
     async def list_provisioned_product_plans(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         PageSize: int = ...,
         PageToken: str = ...,
-        AccessLevelFilter: AccessLevelFilterTypeDef = ...
+        AccessLevelFilter: AccessLevelFilterTypeDef = ...,
     ) -> ListProvisionedProductPlansOutputTypeDef:
         """
         Lists the plans for the specified provisioned product or all plans to which the
         user has
         access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_provisioned_product_plans)
@@ -1066,15 +1066,15 @@
 
     async def list_provisioning_artifacts_for_service_action(
         self,
         *,
         ServiceActionId: str,
         PageSize: int = ...,
         PageToken: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> ListProvisioningArtifactsForServiceActionOutputTypeDef:
         """
         Lists all provisioning artifacts (also known as versions) for the specified
         self-service
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_provisioning_artifacts_for_service_action)
@@ -1084,30 +1084,30 @@
     async def list_record_history(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListRecordHistoryOutputTypeDef:
         """
         Lists the specified requests or all performed requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_record_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_record_history)
         """
 
     async def list_resources_for_tag_option(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListResourcesForTagOptionOutputTypeDef:
         """
         Lists the resources associated with the specified TagOption.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_resources_for_tag_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_resources_for_tag_option)
         """
@@ -1125,15 +1125,15 @@
     async def list_service_actions_for_provisioning_artifact(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         PageSize: int = ...,
         PageToken: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> ListServiceActionsForProvisioningArtifactOutputTypeDef:
         """
         Returns a paginated list of self-service actions associated with the specified
         Product ID and Provisioning Artifact
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_service_actions_for_provisioning_artifact)
@@ -1142,15 +1142,15 @@
 
     async def list_stack_instances_for_provisioned_product(
         self,
         *,
         ProvisionedProductId: str,
         AcceptLanguage: str = ...,
         PageToken: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> ListStackInstancesForProvisionedProductOutputTypeDef:
         """
         Returns summary information about stack instances that are associated with the
         specified `CFN_STACKSET` type provisioned
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_stack_instances_for_provisioned_product)
@@ -1158,15 +1158,15 @@
         """
 
     async def list_tag_options(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ListTagOptionsOutputTypeDef:
         """
         Lists the specified TagOptions or all TagOptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_tag_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#list_tag_options)
         """
@@ -1176,15 +1176,15 @@
         *,
         WorkflowToken: str,
         RecordId: str,
         Status: EngineWorkflowStatusType,
         IdempotencyToken: str,
         FailureReason: str = ...,
         ResourceIdentifier: EngineWorkflowResourceIdentifierTypeDef = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
+        Outputs: Sequence[RecordOutputTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Notifies the result of the provisioning engine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_provision_product_engine_workflow_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#notify_provision_product_engine_workflow_result)
         """
@@ -1192,15 +1192,15 @@
     async def notify_terminate_provisioned_product_engine_workflow_result(
         self,
         *,
         WorkflowToken: str,
         RecordId: str,
         Status: EngineWorkflowStatusType,
         IdempotencyToken: str,
-        FailureReason: str = ...
+        FailureReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Notifies the result of the terminate engine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_terminate_provisioned_product_engine_workflow_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#notify_terminate_provisioned_product_engine_workflow_result)
         """
@@ -1209,15 +1209,15 @@
         self,
         *,
         WorkflowToken: str,
         RecordId: str,
         Status: EngineWorkflowStatusType,
         IdempotencyToken: str,
         FailureReason: str = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
+        Outputs: Sequence[RecordOutputTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Notifies the result of the update engine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_update_provisioned_product_engine_workflow_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#notify_update_provisioned_product_engine_workflow_result)
         """
@@ -1233,44 +1233,44 @@
         ProvisioningArtifactId: str = ...,
         ProvisioningArtifactName: str = ...,
         PathId: str = ...,
         PathName: str = ...,
         ProvisioningParameters: Sequence[ProvisioningParameterTypeDef] = ...,
         ProvisioningPreferences: ProvisioningPreferencesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        NotificationArns: Sequence[str] = ...
+        NotificationArns: Sequence[str] = ...,
     ) -> ProvisionProductOutputTypeDef:
         """
         Provisions the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.provision_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#provision_product)
         """
 
     async def reject_portfolio_share(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PortfolioShareType: PortfolioShareTypeType = ...
+        PortfolioShareType: PortfolioShareTypeType = ...,
     ) -> Dict[str, Any]:
         """
         Rejects an offer to share the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.reject_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#reject_portfolio_share)
         """
 
     async def scan_provisioned_products(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> ScanProvisionedProductsOutputTypeDef:
         """
         Lists the provisioned products that are available (not terminated).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.scan_provisioned_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#scan_provisioned_products)
         """
@@ -1279,15 +1279,15 @@
         self,
         *,
         AcceptLanguage: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         PageSize: int = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> SearchProductsOutputTypeDef:
         """
         Gets information about the products to which the caller has access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.search_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#search_products)
         """
@@ -1298,15 +1298,15 @@
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         PageToken: str = ...,
         PageSize: int = ...,
-        ProductSource: Literal["ACCOUNT"] = ...
+        ProductSource: Literal["ACCOUNT"] = ...,
     ) -> SearchProductsAsAdminOutputTypeDef:
         """
         Gets information about the products for the specified portfolio or all products.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.search_products_as_admin)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#search_products_as_admin)
         """
@@ -1316,15 +1316,15 @@
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         Filters: Mapping[Literal["SearchQuery"], Sequence[str]] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         PageSize: int = ...,
-        PageToken: str = ...
+        PageToken: str = ...,
     ) -> SearchProvisionedProductsOutputTypeDef:
         """
         Gets information about the provisioned products that meet the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.search_provisioned_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#search_provisioned_products)
@@ -1334,15 +1334,15 @@
         self,
         *,
         TerminateToken: str,
         ProvisionedProductName: str = ...,
         ProvisionedProductId: str = ...,
         IgnoreErrors: bool = ...,
         AcceptLanguage: str = ...,
-        RetainPhysicalResources: bool = ...
+        RetainPhysicalResources: bool = ...,
     ) -> TerminateProvisionedProductOutputTypeDef:
         """
         Terminates the specified provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.terminate_provisioned_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#terminate_provisioned_product)
         """
@@ -1362,15 +1362,15 @@
         *,
         Id: str,
         AcceptLanguage: str = ...,
         DisplayName: str = ...,
         Description: str = ...,
         ProviderName: str = ...,
         AddTags: Sequence[TagTypeDef] = ...,
-        RemoveTags: Sequence[str] = ...
+        RemoveTags: Sequence[str] = ...,
     ) -> UpdatePortfolioOutputTypeDef:
         """
         Updates the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_portfolio)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_portfolio)
         """
@@ -1379,15 +1379,15 @@
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         AccountId: str = ...,
         OrganizationNode: OrganizationNodeTypeDef = ...,
         ShareTagOptions: bool = ...,
-        SharePrincipals: bool = ...
+        SharePrincipals: bool = ...,
     ) -> UpdatePortfolioShareOutputTypeDef:
         """
         Updates the specified portfolio share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_portfolio_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_portfolio_share)
         """
@@ -1402,15 +1402,15 @@
         Description: str = ...,
         Distributor: str = ...,
         SupportDescription: str = ...,
         SupportEmail: str = ...,
         SupportUrl: str = ...,
         AddTags: Sequence[TagTypeDef] = ...,
         RemoveTags: Sequence[str] = ...,
-        SourceConnection: SourceConnectionTypeDef = ...
+        SourceConnection: SourceConnectionTypeDef = ...,
     ) -> UpdateProductOutputTypeDef:
         """
         Updates the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_product)
         """
@@ -1426,30 +1426,30 @@
         ProductName: str = ...,
         ProvisioningArtifactId: str = ...,
         ProvisioningArtifactName: str = ...,
         PathId: str = ...,
         PathName: str = ...,
         ProvisioningParameters: Sequence[UpdateProvisioningParameterTypeDef] = ...,
         ProvisioningPreferences: UpdateProvisioningPreferencesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateProvisionedProductOutputTypeDef:
         """
         Requests updates to the configuration of the specified provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_provisioned_product)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_provisioned_product)
         """
 
     async def update_provisioned_product_properties(
         self,
         *,
         ProvisionedProductId: str,
         ProvisionedProductProperties: Mapping[PropertyKeyType, str],
         IdempotencyToken: str,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> UpdateProvisionedProductPropertiesOutputTypeDef:
         """
         Requests updates to the properties of the specified provisioned product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_provisioned_product_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_provisioned_product_properties)
         """
@@ -1459,15 +1459,15 @@
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
         Name: str = ...,
         Description: str = ...,
         Active: bool = ...,
-        Guidance: ProvisioningArtifactGuidanceType = ...
+        Guidance: ProvisioningArtifactGuidanceType = ...,
     ) -> UpdateProvisioningArtifactOutputTypeDef:
         """
         Updates the specified provisioning artifact (also known as a version) for the
         specified
         product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_provisioning_artifact)
@@ -1477,15 +1477,15 @@
     async def update_service_action(
         self,
         *,
         Id: str,
         Name: str = ...,
         Definition: Mapping[ServiceActionDefinitionKeyType, str] = ...,
         Description: str = ...,
-        AcceptLanguage: str = ...
+        AcceptLanguage: str = ...,
     ) -> UpdateServiceActionOutputTypeDef:
         """
         Updates a self-service action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.update_service_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/client/#update_service_action)
         """
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/literals.py` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/literals.py`

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
     "AccessLevelFilterKeyType",
     "AccessStatusType",
     "ChangeActionType",
     "CopyOptionType",
     "CopyProductStatusType",
     "DescribePortfolioShareTypeType",
@@ -77,15 +76,14 @@
     "ServiceCatalogServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessLevelFilterKeyType = Literal["Account", "Role", "User"]
 AccessStatusType = Literal["DISABLED", "ENABLED", "UNDER_CHANGE"]
 ChangeActionType = Literal["ADD", "MODIFY", "REMOVE"]
 CopyOptionType = Literal["CopyTags"]
 CopyProductStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 DescribePortfolioShareTypeType = Literal[
     "ACCOUNT", "ORGANIZATION", "ORGANIZATIONAL_UNIT", "ORGANIZATION_MEMBER_ACCOUNT"
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/literals.pyi` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/paginator.py` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAcceptedPortfolioSharesPaginator",
     "ListConstraintsForPortfolioPaginator",
     "ListLaunchPathsPaginator",
     "ListOrganizationPortfolioAccessPaginator",
     "ListPortfoliosPaginator",
     "ListPortfoliosForProductPaginator",
@@ -108,15 +107,14 @@
     "ListServiceActionsPaginator",
     "ListServiceActionsForProvisioningArtifactPaginator",
     "ListTagOptionsPaginator",
     "ScanProvisionedProductsPaginator",
     "SearchProductsAsAdminPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -130,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         PortfolioShareType: PortfolioShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAcceptedPortfolioSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listacceptedportfoliosharespaginator)
         """
 
 
@@ -150,15 +148,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConstraintsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listconstraintsforportfoliopaginator)
         """
 
 
@@ -169,15 +167,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchPathsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listlaunchpathspaginator)
         """
 
 
@@ -189,15 +187,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationPortfolioAccessOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listorganizationportfolioaccesspaginator)
         """
 
 
@@ -223,15 +221,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPortfoliosForProductOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliosforproductpaginator)
         """
 
 
@@ -242,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrincipalsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprincipalsforportfoliopaginator)
         """
 
 
@@ -262,15 +260,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProvisionedProductPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisionedproductplanspaginator)
         """
 
 
@@ -281,15 +279,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceActionId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisioningartifactsforserviceactionpaginator)
         """
 
 
@@ -301,15 +299,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecordHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listrecordhistorypaginator)
         """
 
 
@@ -320,15 +318,15 @@
     """
 
     def paginate(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesForTagOptionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listresourcesfortagoptionpaginator)
         """
 
 
@@ -355,15 +353,15 @@
 
     def paginate(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionsforprovisioningartifactpaginator)
         """
 
 
@@ -373,15 +371,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTagOptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
         """
 
 
@@ -392,15 +390,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScanProvisionedProductsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#scanprovisionedproductspaginator)
         """
 
 
@@ -415,13 +413,13 @@
         *,
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         ProductSource: Literal["ACCOUNT"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchProductsAsAdminOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#searchproductsasadminpaginator)
         """
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/paginator.pyi` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         PortfolioShareType: PortfolioShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAcceptedPortfolioSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listacceptedportfoliosharespaginator)
         """
 
 class ListConstraintsForPortfolioPaginator(AioPaginator):
@@ -145,15 +145,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConstraintsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listconstraintsforportfoliopaginator)
         """
 
 class ListLaunchPathsPaginator(AioPaginator):
@@ -163,15 +163,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLaunchPathsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listlaunchpathspaginator)
         """
 
 class ListOrganizationPortfolioAccessPaginator(AioPaginator):
@@ -182,15 +182,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOrganizationPortfolioAccessOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listorganizationportfolioaccesspaginator)
         """
 
 class ListPortfoliosPaginator(AioPaginator):
@@ -214,15 +214,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPortfoliosForProductOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliosforproductpaginator)
         """
 
 class ListPrincipalsForPortfolioPaginator(AioPaginator):
@@ -232,15 +232,15 @@
     """
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrincipalsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprincipalsforportfoliopaginator)
         """
 
 class ListProvisionedProductPlansPaginator(AioPaginator):
@@ -251,15 +251,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProvisionedProductPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisionedproductplanspaginator)
         """
 
 class ListProvisioningArtifactsForServiceActionPaginator(AioPaginator):
@@ -269,15 +269,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceActionId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisioningartifactsforserviceactionpaginator)
         """
 
 class ListRecordHistoryPaginator(AioPaginator):
@@ -288,15 +288,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecordHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listrecordhistorypaginator)
         """
 
 class ListResourcesForTagOptionPaginator(AioPaginator):
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesForTagOptionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listresourcesfortagoptionpaginator)
         """
 
 class ListServiceActionsPaginator(AioPaginator):
@@ -339,15 +339,15 @@
 
     def paginate(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionsforprovisioningartifactpaginator)
         """
 
 class ListTagOptionsPaginator(AioPaginator):
@@ -356,15 +356,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTagOptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
         """
 
 class ScanProvisionedProductsPaginator(AioPaginator):
@@ -374,15 +374,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ScanProvisionedProductsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#scanprovisionedproductspaginator)
         """
 
 class SearchProductsAsAdminPaginator(AioPaginator):
@@ -396,13 +396,13 @@
         *,
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         ProductSource: Literal["ACCOUNT"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchProductsAsAdminOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#searchproductsasadminpaginator)
         """
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/type_defs.py` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptPortfolioShareInputRequestTypeDef",
     "AccessLevelFilterTypeDef",
     "AssociateBudgetWithResourceInputRequestTypeDef",
     "AssociatePrincipalWithPortfolioInputRequestTypeDef",
     "AssociateProductWithPortfolioInputRequestTypeDef",
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog/type_defs.pyi` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/PKG-INFO` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServiceCatalog 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServiceCatalog 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/
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
 
 <a id="types-aiobotocore-servicecatalog"></a>
 
 # types-aiobotocore-servicecatalog
 
 [![PyPI - types-aiobotocore-servicecatalog](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog)](https://pepy.tech/project/types-aiobotocore-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceCatalog 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[aiobotocore.ServiceCatalog 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [types-aiobotocore-servicecatalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicecatalog-2.9.0/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt` & `types-aiobotocore-servicecatalog-2.9.1/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

