# Comparing `tmp/types-aiobotocore-service-quotas-2.9.0.tar.gz` & `tmp/types-aiobotocore-service-quotas-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-service-quotas-2.9.0.tar", last modified: Wed Dec 13 20:00:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-service-quotas-2.9.1.tar", last modified: Thu Jan 18 01:21:48 2024, max compression
```

## Comparing `types-aiobotocore-service-quotas-2.9.0.tar` & `types-aiobotocore-service-quotas-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.489146 types-aiobotocore-service-quotas-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2023-12-13 20:00:29.489146 types-aiobotocore-service-quotas-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:29.489146 types-aiobotocore-service-quotas-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.489146 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10663 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16649 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:16.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:29.489146 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2023-12-13 20:00:29.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:29.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:29.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:29.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:29.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:29.000000 types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.005038 types-aiobotocore-service-quotas-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:45.000000 types-aiobotocore-service-quotas-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-01-18 01:21:48.005038 types-aiobotocore-service-quotas-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-01-18 01:17:45.000000 types-aiobotocore-service-quotas-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:48.005038 types-aiobotocore-service-quotas-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-18 01:17:45.000000 types-aiobotocore-service-quotas-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.001038 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-01-18 01:17:45.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-01-18 01:17:45.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16649 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16649 2024-01-18 01:17:46.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:45.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:48.005038 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-01-18 01:21:47.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:47.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:47.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:47.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:47.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:47.000000 types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/LICENSE` & `types-aiobotocore-service-quotas-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-service-quotas-2.9.0/PKG-INFO` & `types-aiobotocore-service-quotas-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
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
 
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceQuotas 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[aiobotocore.ServiceQuotas 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/README.md` & `types-aiobotocore-service-quotas-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceQuotas 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[aiobotocore.ServiceQuotas 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/setup.py` & `types-aiobotocore-service-quotas-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-service-quotas",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServiceQuotas 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ServiceQuotas 2.9.1 service generated with"
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
     keywords="aiobotocore service-quotas type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_service_quotas": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/__init__.py` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListServiceQuotaIncreaseRequestsInTemplatePaginator,
     ListServiceQuotasPaginator,
     ListServicesPaginator,
 )
 
 Client = ServiceQuotasClient
 
-
 __all__ = (
     "Client",
     "ListAWSDefaultServiceQuotasPaginator",
     "ListRequestedServiceQuotaChangeHistoryByQuotaPaginator",
     "ListRequestedServiceQuotaChangeHistoryPaginator",
     "ListServiceQuotaIncreaseRequestsInTemplatePaginator",
     "ListServiceQuotasPaginator",
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/__init__.pyi` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/__main__.py` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceQuotas 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ServiceQuotas 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas\nOther"
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

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/client.py` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ServiceQuotasClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -226,15 +225,15 @@
     async def list_requested_service_quota_change_history(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuotaRequestedAtLevel: AppliedLevelEnumType = ...
+        QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
     ) -> ListRequestedServiceQuotaChangeHistoryResponseTypeDef:
         """
         Retrieves the quota increase requests for the specified Amazon Web Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_requested_service_quota_change_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_requested_service_quota_change_history)
         """
@@ -243,30 +242,30 @@
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuotaRequestedAtLevel: AppliedLevelEnumType = ...
+        QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
     ) -> ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef:
         """
         Retrieves the quota increase requests for the specified quota.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_requested_service_quota_change_history_by_quota)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_requested_service_quota_change_history_by_quota)
         """
 
     async def list_service_quota_increase_requests_in_template(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef:
         """
         Lists the quota increase requests in the specified quota request template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_service_quota_increase_requests_in_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_service_quota_increase_requests_in_template)
         """
@@ -274,15 +273,15 @@
     async def list_service_quotas(
         self,
         *,
         ServiceCode: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         QuotaCode: str = ...,
-        QuotaAppliedAtLevel: AppliedLevelEnumType = ...
+        QuotaAppliedAtLevel: AppliedLevelEnumType = ...,
     ) -> ListServiceQuotasResponseTypeDef:
         """
         Lists the applied quota values for the specified Amazon Web Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_service_quotas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_service_quotas)
         """
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/client.pyi` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     async def list_requested_service_quota_change_history(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuotaRequestedAtLevel: AppliedLevelEnumType = ...
+        QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
     ) -> ListRequestedServiceQuotaChangeHistoryResponseTypeDef:
         """
         Retrieves the quota increase requests for the specified Amazon Web Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_requested_service_quota_change_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_requested_service_quota_change_history)
         """
@@ -239,30 +239,30 @@
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        QuotaRequestedAtLevel: AppliedLevelEnumType = ...
+        QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
     ) -> ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef:
         """
         Retrieves the quota increase requests for the specified quota.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_requested_service_quota_change_history_by_quota)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_requested_service_quota_change_history_by_quota)
         """
 
     async def list_service_quota_increase_requests_in_template(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef:
         """
         Lists the quota increase requests in the specified quota request template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_service_quota_increase_requests_in_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_service_quota_increase_requests_in_template)
         """
@@ -270,15 +270,15 @@
     async def list_service_quotas(
         self,
         *,
         ServiceCode: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         QuotaCode: str = ...,
-        QuotaAppliedAtLevel: AppliedLevelEnumType = ...
+        QuotaAppliedAtLevel: AppliedLevelEnumType = ...,
     ) -> ListServiceQuotasResponseTypeDef:
         """
         Lists the applied quota values for the specified Amazon Web Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client.list_service_quotas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/client/#list_service_quotas)
         """
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/literals.py` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AppliedLevelEnumType",
     "ErrorCodeType",
     "ListAWSDefaultServiceQuotasPaginatorName",
     "ListRequestedServiceQuotaChangeHistoryByQuotaPaginatorName",
     "ListRequestedServiceQuotaChangeHistoryPaginatorName",
     "ListServiceQuotaIncreaseRequestsInTemplatePaginatorName",
@@ -36,15 +35,14 @@
     "ServiceQuotasServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AppliedLevelEnumType = Literal["ACCOUNT", "ALL", "RESOURCE"]
 ErrorCodeType = Literal[
     "DEPENDENCY_ACCESS_DENIED_ERROR",
     "DEPENDENCY_SERVICE_ERROR",
     "DEPENDENCY_THROTTLING_ERROR",
     "SERVICE_QUOTA_NOT_AVAILABLE_ERROR",
 ]
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/literals.pyi` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/paginator.py` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "ListRequestedServiceQuotaChangeHistoryPaginator",
     "ListRequestedServiceQuotaChangeHistoryByQuotaPaginator",
     "ListServiceQuotaIncreaseRequestsInTemplatePaginator",
     "ListServiceQuotasPaginator",
     "ListServicesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -90,15 +89,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
         QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
 
@@ -111,15 +110,15 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
         QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
 
@@ -130,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
 
@@ -150,15 +149,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str = ...,
         QuotaAppliedAtLevel: AppliedLevelEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaspaginator)
         """
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/paginator.pyi` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
         QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
 class ListRequestedServiceQuotaChangeHistoryByQuotaPaginator(AioPaginator):
@@ -106,15 +106,15 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
         QuotaRequestedAtLevel: AppliedLevelEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
 class ListServiceQuotaIncreaseRequestsInTemplatePaginator(AioPaginator):
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
 class ListServiceQuotasPaginator(AioPaginator):
@@ -143,15 +143,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str = ...,
         QuotaAppliedAtLevel: AppliedLevelEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaspaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/type_defs.py` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/type_defs.py`

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
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas/type_defs.pyi` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/PKG-INFO` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
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
 
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceQuotas 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[aiobotocore.ServiceQuotas 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-service-quotas-2.9.0/types_aiobotocore_service_quotas.egg-info/SOURCES.txt` & `types-aiobotocore-service-quotas-2.9.1/types_aiobotocore_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

