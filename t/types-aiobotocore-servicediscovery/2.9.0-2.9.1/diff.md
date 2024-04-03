# Comparing `tmp/types-aiobotocore-servicediscovery-2.9.0.tar.gz` & `tmp/types-aiobotocore-servicediscovery-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicediscovery-2.9.0.tar", last modified: Wed Dec 13 20:00:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicediscovery-2.9.1.tar", last modified: Thu Jan 18 01:21:49 2024, max compression
```

## Comparing `types-aiobotocore-servicediscovery-2.9.0.tar` & `types-aiobotocore-servicediscovery-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:30.617136 types-aiobotocore-servicediscovery-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2023-12-13 20:00:30.617136 types-aiobotocore-servicediscovery-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:30.617136 types-aiobotocore-servicediscovery-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:30.617136 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25277 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25893 2023-12-13 19:56:25.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25892 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:24.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:30.617136 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2023-12-13 20:00:30.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 20:00:30.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:30.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:30.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:30.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 20:00:30.000000 types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:49.025034 types-aiobotocore-servicediscovery-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-01-18 01:21:49.025034 types-aiobotocore-servicediscovery-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:49.025034 types-aiobotocore-servicediscovery-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:49.025034 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25286 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25283 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25892 2024-01-18 01:17:56.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25892 2024-01-18 01:17:56.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:55.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:49.025034 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-01-18 01:21:48.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:21:49.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:48.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:48.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:48.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:48.000000 types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/LICENSE` & `types-aiobotocore-servicediscovery-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-servicediscovery-2.9.0/PKG-INFO` & `types-aiobotocore-servicediscovery-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
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
 
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceDiscovery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[aiobotocore.ServiceDiscovery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/README.md` & `types-aiobotocore-servicediscovery-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceDiscovery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[aiobotocore.ServiceDiscovery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/setup.py` & `types-aiobotocore-servicediscovery-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicediscovery",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServiceDiscovery 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ServiceDiscovery 2.9.1 service generated with"
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
     keywords="aiobotocore servicediscovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_servicediscovery": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/__init__.py` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListNamespacesPaginator,
     ListOperationsPaginator,
     ListServicesPaginator,
 )
 
 Client = ServiceDiscoveryClient
 
-
 __all__ = (
     "Client",
     "ListInstancesPaginator",
     "ListNamespacesPaginator",
     "ListOperationsPaginator",
     "ListServicesPaginator",
     "ServiceDiscoveryClient",
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/__init__.pyi` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/__main__.py` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceDiscovery 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ServiceDiscovery 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/client.py` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ServiceDiscoveryClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -138,15 +137,15 @@
 
     async def create_http_namespace(
         self,
         *,
         Name: str,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHttpNamespaceResponseTypeDef:
         """
         Creates an HTTP namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_http_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#create_http_namespace)
         """
@@ -155,15 +154,15 @@
         self,
         *,
         Name: str,
         Vpc: str,
         CreatorRequestId: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Properties: PrivateDnsNamespacePropertiesTypeDef = ...
+        Properties: PrivateDnsNamespacePropertiesTypeDef = ...,
     ) -> CreatePrivateDnsNamespaceResponseTypeDef:
         """
         Creates a private namespace based on DNS, which is visible only inside a
         specified Amazon
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_private_dns_namespace)
@@ -173,15 +172,15 @@
     async def create_public_dns_namespace(
         self,
         *,
         Name: str,
         CreatorRequestId: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Properties: PublicDnsNamespacePropertiesTypeDef = ...
+        Properties: PublicDnsNamespacePropertiesTypeDef = ...,
     ) -> CreatePublicDnsNamespaceResponseTypeDef:
         """
         Creates a public namespace based on DNS, which is visible on the internet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_public_dns_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#create_public_dns_namespace)
         """
@@ -193,15 +192,15 @@
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
         DnsConfig: DnsConfigTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Type: Literal["HTTP"] = ...
+        Type: Literal["HTTP"] = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#create_service)
         """
@@ -238,15 +237,15 @@
         self,
         *,
         NamespaceName: str,
         ServiceName: str,
         MaxResults: int = ...,
         QueryParameters: Mapping[str, str] = ...,
         OptionalParameters: Mapping[str, str] = ...,
-        HealthStatus: HealthStatusFilterType = ...
+        HealthStatus: HealthStatusFilterType = ...,
     ) -> DiscoverInstancesResponseTypeDef:
         """
         Discovers registered instances for a specified namespace and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.discover_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#discover_instances)
         """
@@ -285,15 +284,15 @@
 
     async def get_instances_health_status(
         self,
         *,
         ServiceId: str,
         Instances: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetInstancesHealthStatusResponseTypeDef:
         """
         Gets the current health status ( `Healthy`, `Unhealthy`, or `Unknown`) of one
         or more instances that are associated with a specified
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.get_instances_health_status)
@@ -339,15 +338,15 @@
         """
 
     async def list_namespaces(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[NamespaceFilterTypeDef] = ...
+        Filters: Sequence[NamespaceFilterTypeDef] = ...,
     ) -> ListNamespacesResponseTypeDef:
         """
         Lists summary information about the namespaces that were created by the current
         Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.list_namespaces)
@@ -355,29 +354,29 @@
         """
 
     async def list_operations(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[OperationFilterTypeDef] = ...
+        Filters: Sequence[OperationFilterTypeDef] = ...,
     ) -> ListOperationsResponseTypeDef:
         """
         Lists operations that match the criteria that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.list_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#list_operations)
         """
 
     async def list_services(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[ServiceFilterTypeDef] = ...
+        Filters: Sequence[ServiceFilterTypeDef] = ...,
     ) -> ListServicesResponseTypeDef:
         """
         Lists summary information for all the services that are associated with one or
         more specified
         namespaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.list_services)
@@ -396,15 +395,15 @@
 
     async def register_instance(
         self,
         *,
         ServiceId: str,
         InstanceId: str,
         Attributes: Mapping[str, str],
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> RegisterInstanceResponseTypeDef:
         """
         Creates or updates one or more records and, optionally, creates a health check
         based on the settings in a specified
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.register_instance)
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/client.pyi` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     async def create_http_namespace(
         self,
         *,
         Name: str,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHttpNamespaceResponseTypeDef:
         """
         Creates an HTTP namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_http_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#create_http_namespace)
         """
@@ -151,15 +151,15 @@
         self,
         *,
         Name: str,
         Vpc: str,
         CreatorRequestId: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Properties: PrivateDnsNamespacePropertiesTypeDef = ...
+        Properties: PrivateDnsNamespacePropertiesTypeDef = ...,
     ) -> CreatePrivateDnsNamespaceResponseTypeDef:
         """
         Creates a private namespace based on DNS, which is visible only inside a
         specified Amazon
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_private_dns_namespace)
@@ -169,15 +169,15 @@
     async def create_public_dns_namespace(
         self,
         *,
         Name: str,
         CreatorRequestId: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Properties: PublicDnsNamespacePropertiesTypeDef = ...
+        Properties: PublicDnsNamespacePropertiesTypeDef = ...,
     ) -> CreatePublicDnsNamespaceResponseTypeDef:
         """
         Creates a public namespace based on DNS, which is visible on the internet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_public_dns_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#create_public_dns_namespace)
         """
@@ -189,15 +189,15 @@
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
         DnsConfig: DnsConfigTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Type: Literal["HTTP"] = ...
+        Type: Literal["HTTP"] = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#create_service)
         """
@@ -234,15 +234,15 @@
         self,
         *,
         NamespaceName: str,
         ServiceName: str,
         MaxResults: int = ...,
         QueryParameters: Mapping[str, str] = ...,
         OptionalParameters: Mapping[str, str] = ...,
-        HealthStatus: HealthStatusFilterType = ...
+        HealthStatus: HealthStatusFilterType = ...,
     ) -> DiscoverInstancesResponseTypeDef:
         """
         Discovers registered instances for a specified namespace and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.discover_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#discover_instances)
         """
@@ -281,15 +281,15 @@
 
     async def get_instances_health_status(
         self,
         *,
         ServiceId: str,
         Instances: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetInstancesHealthStatusResponseTypeDef:
         """
         Gets the current health status ( `Healthy`, `Unhealthy`, or `Unknown`) of one
         or more instances that are associated with a specified
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.get_instances_health_status)
@@ -335,15 +335,15 @@
         """
 
     async def list_namespaces(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[NamespaceFilterTypeDef] = ...
+        Filters: Sequence[NamespaceFilterTypeDef] = ...,
     ) -> ListNamespacesResponseTypeDef:
         """
         Lists summary information about the namespaces that were created by the current
         Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.list_namespaces)
@@ -351,29 +351,29 @@
         """
 
     async def list_operations(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[OperationFilterTypeDef] = ...
+        Filters: Sequence[OperationFilterTypeDef] = ...,
     ) -> ListOperationsResponseTypeDef:
         """
         Lists operations that match the criteria that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.list_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/client/#list_operations)
         """
 
     async def list_services(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: Sequence[ServiceFilterTypeDef] = ...
+        Filters: Sequence[ServiceFilterTypeDef] = ...,
     ) -> ListServicesResponseTypeDef:
         """
         Lists summary information for all the services that are associated with one or
         more specified
         namespaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.list_services)
@@ -392,15 +392,15 @@
 
     async def register_instance(
         self,
         *,
         ServiceId: str,
         InstanceId: str,
         Attributes: Mapping[str, str],
-        CreatorRequestId: str = ...
+        CreatorRequestId: str = ...,
     ) -> RegisterInstanceResponseTypeDef:
         """
         Creates or updates one or more records and, optionally, creates a health check
         based on the settings in a specified
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Client.register_instance)
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/literals.py` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/literals.py`

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
     "CustomHealthStatusType",
     "FilterConditionType",
     "HealthCheckTypeType",
     "HealthStatusFilterType",
     "HealthStatusType",
     "ListInstancesPaginatorName",
@@ -44,15 +43,14 @@
     "ServiceDiscoveryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CustomHealthStatusType = Literal["HEALTHY", "UNHEALTHY"]
 FilterConditionType = Literal["BEGINS_WITH", "BETWEEN", "EQ", "IN"]
 HealthCheckTypeType = Literal["HTTP", "HTTPS", "TCP"]
 HealthStatusFilterType = Literal["ALL", "HEALTHY", "HEALTHY_OR_ELSE_ALL", "UNHEALTHY"]
 HealthStatusType = Literal["HEALTHY", "UNHEALTHY", "UNKNOWN"]
 ListInstancesPaginatorName = Literal["list_instances"]
 ListNamespacesPaginatorName = Literal["list_namespaces"]
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/literals.pyi` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/paginator.py` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 __all__ = (
     "ListInstancesPaginator",
     "ListNamespacesPaginator",
     "ListOperationsPaginator",
     "ListServicesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -82,15 +81,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 
@@ -100,15 +99,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
         """
 
 
@@ -118,13 +117,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/paginator.pyi` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 class ListOperationsPaginator(AioPaginator):
@@ -95,15 +95,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
@@ -112,13 +112,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListServicesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/type_defs.py` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery/type_defs.pyi` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/PKG-INFO` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
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
 
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceDiscovery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[aiobotocore.ServiceDiscovery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-servicediscovery-2.9.0/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt` & `types-aiobotocore-servicediscovery-2.9.1/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

