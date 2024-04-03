# Comparing `tmp/types-aiobotocore-elastictranscoder-2.9.0.tar.gz` & `tmp/types-aiobotocore-elastictranscoder-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastictranscoder-2.9.0.tar", last modified: Wed Dec 13 19:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastictranscoder-2.9.1.tar", last modified: Thu Jan 18 01:20:39 2024, max compression
```

## Comparing `types-aiobotocore-elastictranscoder-2.9.0.tar` & `types-aiobotocore-elastictranscoder-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.941765 types-aiobotocore-elastictranscoder-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2023-12-13 19:59:14.941765 types-aiobotocore-elastictranscoder-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13089 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:14.941765 types-aiobotocore-elastictranscoder-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.941765 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18598 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18594 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29039 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29038 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:46.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-12-13 19:45:47.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:14.941765 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2023-12-13 19:59:14.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-13 19:59:14.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:14.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:14.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:14.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:59:14.000000 types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.765347 types-aiobotocore-elastictranscoder-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-01-18 01:20:39.761347 types-aiobotocore-elastictranscoder-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13089 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:39.765347 types-aiobotocore-elastictranscoder-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.761347 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18598 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29038 2024-01-18 01:07:43.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29038 2024-01-18 01:07:43.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-18 01:07:42.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:39.761347 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-01-18 01:20:39.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-18 01:20:39.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:39.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:39.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:39.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:39.000000 types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/LICENSE` & `types-aiobotocore-elastictranscoder-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
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
 
 <a id="types-aiobotocore-elastictranscoder"></a>
 
 # types-aiobotocore-elastictranscoder
 
 [![PyPI - types-aiobotocore-elastictranscoder](https://img.shields.io/pypi/v/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastictranscoder)](https://pepy.tech/project/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticTranscoder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[aiobotocore.ElasticTranscoder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/README.md` & `types-aiobotocore-elastictranscoder-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastictranscoder)](https://pepy.tech/project/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticTranscoder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[aiobotocore.ElasticTranscoder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/setup.py` & `types-aiobotocore-elastictranscoder-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastictranscoder",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticTranscoder 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElasticTranscoder 2.9.1 service generated with"
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
     keywords="aiobotocore elastictranscoder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elastictranscoder": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/__init__.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     ListPipelinesPaginator,
     ListPresetsPaginator,
 )
 from .waiter import JobCompleteWaiter
 
 Client = ElasticTranscoderClient
 
-
 __all__ = (
     "Client",
     "ElasticTranscoderClient",
     "JobCompleteWaiter",
     "ListJobsByPipelinePaginator",
     "ListJobsByStatusPaginator",
     "ListPipelinesPaginator",
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/__init__.pyi` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/__main__.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticTranscoder 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElasticTranscoder 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/client.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,37 +54,33 @@
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticTranscoderClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IncompatibleVersionException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ElasticTranscoderClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/)
     """
 
     meta: ClientMeta
@@ -128,15 +124,15 @@
         PipelineId: str,
         Input: JobInputTypeDef = ...,
         Inputs: Sequence[JobInputTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
-        UserMetadata: Mapping[str, str] = ...
+        UserMetadata: Mapping[str, str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         When you create a job, Elastic Transcoder returns JSON data that includes the
         values that you specified plus information about the job that is
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_job)
@@ -149,15 +145,15 @@
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
         ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_pipeline)
         """
@@ -166,15 +162,15 @@
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
         Video: VideoParametersTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
-        Thumbnails: ThumbnailsTypeDef = ...
+        Thumbnails: ThumbnailsTypeDef = ...,
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_preset)
         """
@@ -294,15 +290,15 @@
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
         ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...,
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/client.pyi` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,31 +56,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("ElasticTranscoderClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IncompatibleVersionException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ElasticTranscoderClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/)
     """
 
     meta: ClientMeta
@@ -124,15 +127,15 @@
         PipelineId: str,
         Input: JobInputTypeDef = ...,
         Inputs: Sequence[JobInputTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
-        UserMetadata: Mapping[str, str] = ...
+        UserMetadata: Mapping[str, str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         When you create a job, Elastic Transcoder returns JSON data that includes the
         values that you specified plus information about the job that is
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_job)
@@ -145,15 +148,15 @@
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
         ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_pipeline)
         """
@@ -162,15 +165,15 @@
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
         Video: VideoParametersTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
-        Thumbnails: ThumbnailsTypeDef = ...
+        Thumbnails: ThumbnailsTypeDef = ...,
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_preset)
         """
@@ -290,15 +293,15 @@
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
         ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...,
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/literals.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "JobCompleteWaiterName",
     "ListJobsByPipelinePaginatorName",
     "ListJobsByStatusPaginatorName",
     "ListPipelinesPaginatorName",
     "ListPresetsPaginatorName",
     "ElasticTranscoderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 JobCompleteWaiterName = Literal["job_complete"]
 ListJobsByPipelinePaginatorName = Literal["list_jobs_by_pipeline"]
 ListJobsByStatusPaginatorName = Literal["list_jobs_by_status"]
 ListPipelinesPaginatorName = Literal["list_pipelines"]
 ListPresetsPaginatorName = Literal["list_presets"]
 ElasticTranscoderServiceName = Literal["elastictranscoder"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/literals.pyi` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/paginator.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListJobsByPipelinePaginator",
     "ListJobsByStatusPaginator",
     "ListPipelinesPaginator",
     "ListPresetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -65,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsByPipelineResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/paginator.pyi` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsByPipelineResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
 class ListJobsByStatusPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/type_defs.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EncryptionTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/type_defs.pyi` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/waiter.py` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder/waiter.pyi` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
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
 
 <a id="types-aiobotocore-elastictranscoder"></a>
 
 # types-aiobotocore-elastictranscoder
 
 [![PyPI - types-aiobotocore-elastictranscoder](https://img.shields.io/pypi/v/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastictranscoder)](https://pepy.tech/project/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticTranscoder 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
+[aiobotocore.ElasticTranscoder 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elastictranscoder-2.9.0/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt` & `types-aiobotocore-elastictranscoder-2.9.1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

