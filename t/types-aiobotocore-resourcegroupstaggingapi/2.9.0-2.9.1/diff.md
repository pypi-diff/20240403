# Comparing `tmp/types-aiobotocore-resourcegroupstaggingapi-2.9.0.tar.gz` & `tmp/types-aiobotocore-resourcegroupstaggingapi-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.9.0.tar", last modified: Wed Dec 13 20:00:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.9.1.tar", last modified: Thu Jan 18 01:21:38 2024, max compression
```

## Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0.tar` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.873237 types-aiobotocore-resourcegroupstaggingapi-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2023-12-13 20:00:18.873237 types-aiobotocore-resourcegroupstaggingapi-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12707 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:18.873237 types-aiobotocore-resourcegroupstaggingapi-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.869238 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12732 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2023-12-13 19:54:42.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2023-12-13 19:54:42.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2023-12-13 19:54:42.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:41.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.873237 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2023-12-13 20:00:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-12-13 20:00:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-13 20:00:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.345081 types-aiobotocore-resourcegroupstaggingapi-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-01-18 01:21:38.345081 types-aiobotocore-resourcegroupstaggingapi-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:38.345081 types-aiobotocore-resourcegroupstaggingapi-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.345081 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-01-18 01:16:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-01-18 01:16:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:17.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.345081 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-01-18 01:21:38.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-18 01:21:38.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:38.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:38.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:38.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-18 01:21:38.000000 types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/LICENSE` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
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
 
 <a id="types-aiobotocore-resourcegroupstaggingapi"></a>
 
 # types-aiobotocore-resourcegroupstaggingapi
 
 [![PyPI - types-aiobotocore-resourcegroupstaggingapi](https://img.shields.io/pypi/v/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroupsTaggingAPI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[aiobotocore.ResourceGroupsTaggingAPI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/README.md` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroupsTaggingAPI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[aiobotocore.ResourceGroupsTaggingAPI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/setup.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resourcegroupstaggingapi",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore resourcegroupstaggingapi type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resourcegroupstaggingapi": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/__init__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     GetResourcesPaginator,
     GetTagKeysPaginator,
     GetTagValuesPaginator,
 )
 
 Client = ResourceGroupsTaggingAPIClient
 
-
 __all__ = (
     "Client",
     "GetComplianceSummaryPaginator",
     "GetResourcesPaginator",
     "GetTagKeysPaginator",
     "GetTagValuesPaginator",
     "ResourceGroupsTaggingAPIClient",
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/__main__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/client.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ResourceGroupsTaggingAPIClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -126,15 +125,15 @@
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
         MaxResults: int = ...,
-        PaginationToken: str = ...
+        PaginationToken: str = ...,
     ) -> GetComplianceSummaryOutputTypeDef:
         """
         Returns a table that shows counts of resources that are noncompliant with their
         tag
         policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_compliance_summary)
@@ -147,15 +146,15 @@
         PaginationToken: str = ...,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         ResourcesPerPage: int = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
-        ResourceARNList: Sequence[str] = ...
+        ResourceARNList: Sequence[str] = ...,
     ) -> GetResourcesOutputTypeDef:
         """
         Returns all the tagged or previously tagged resources that are located in the
         specified Amazon Web Services Region for the
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_resources)
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/client.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
         MaxResults: int = ...,
-        PaginationToken: str = ...
+        PaginationToken: str = ...,
     ) -> GetComplianceSummaryOutputTypeDef:
         """
         Returns a table that shows counts of resources that are noncompliant with their
         tag
         policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_compliance_summary)
@@ -143,15 +143,15 @@
         PaginationToken: str = ...,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         ResourcesPerPage: int = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
-        ResourceARNList: Sequence[str] = ...
+        ResourceARNList: Sequence[str] = ...,
     ) -> GetResourcesOutputTypeDef:
         """
         Returns all the tagged or previously tagged resources that are located in the
         specified Amazon Web Services Region for the
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_resources)
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/literals.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/literals.py`

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
     "ErrorCodeType",
     "GetComplianceSummaryPaginatorName",
     "GetResourcesPaginatorName",
     "GetTagKeysPaginatorName",
     "GetTagValuesPaginatorName",
     "GroupByAttributeType",
@@ -31,15 +30,14 @@
     "ResourceGroupsTaggingAPIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ErrorCodeType = Literal["InternalServiceException", "InvalidParameterException"]
 GetComplianceSummaryPaginatorName = Literal["get_compliance_summary"]
 GetResourcesPaginatorName = Literal["get_resources"]
 GetTagKeysPaginatorName = Literal["get_tag_keys"]
 GetTagValuesPaginatorName = Literal["get_tag_values"]
 GroupByAttributeType = Literal["REGION", "RESOURCE_TYPE", "TARGET_ID"]
 TargetIdTypeType = Literal["ACCOUNT", "OU", "ROOT"]
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/literals.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/paginator.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 __all__ = (
     "GetComplianceSummaryPaginator",
     "GetResourcesPaginator",
     "GetTagKeysPaginator",
     "GetTagValuesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -70,15 +69,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 
@@ -93,15 +92,15 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 class GetResourcesPaginator(AioPaginator):
@@ -89,15 +89,15 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 class GetTagKeysPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/type_defs.py` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/type_defs.py`

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
     "ComplianceDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "FailureInfoTypeDef",
     "PaginatorConfigTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
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
 
 <a id="types-aiobotocore-resourcegroupstaggingapi"></a>
 
 # types-aiobotocore-resourcegroupstaggingapi
 
 [![PyPI - types-aiobotocore-resourcegroupstaggingapi](https://img.shields.io/pypi/v/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroupsTaggingAPI 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[aiobotocore.ResourceGroupsTaggingAPI 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.9.0/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `types-aiobotocore-resourcegroupstaggingapi-2.9.1/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

