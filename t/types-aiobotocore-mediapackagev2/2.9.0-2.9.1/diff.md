# Comparing `tmp/types-aiobotocore-mediapackagev2-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediapackagev2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackagev2-2.9.0.tar", last modified: Wed Dec 13 19:59:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackagev2-2.9.1.tar", last modified: Thu Jan 18 01:21:16 2024, max compression
```

## Comparing `types-aiobotocore-mediapackagev2-2.9.0.tar` & `types-aiobotocore-mediapackagev2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.229453 types-aiobotocore-mediapackagev2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2023-12-13 19:59:54.229453 types-aiobotocore-mediapackagev2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:54.229453 types-aiobotocore-mediapackagev2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.229453 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22005 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22001 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21896 2023-12-13 19:50:18.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21895 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:54.229453 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2023-12-13 19:59:54.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 19:59:54.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:54.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:54.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:54.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 19:59:54.000000 types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.065182 types-aiobotocore-mediapackagev2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-01-18 01:21:16.065182 types-aiobotocore-mediapackagev2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:16.065182 types-aiobotocore-mediapackagev2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.065182 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22009 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21895 2024-01-18 01:12:00.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21895 2024-01-18 01:12:00.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:16.065182 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-01-18 01:21:16.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:16.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:16.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:16.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:16.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:16.000000 types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/LICENSE` & `types-aiobotocore-mediapackagev2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/PKG-INFO` & `types-aiobotocore-mediapackagev2-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackagev2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.mediapackagev2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.mediapackagev2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/
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
 
 <a id="types-aiobotocore-mediapackagev2"></a>
 
 # types-aiobotocore-mediapackagev2
 
 [![PyPI - types-aiobotocore-mediapackagev2](https://img.shields.io/pypi/v/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackagev2)](https://pepy.tech/project/types-aiobotocore-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mediapackagev2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[aiobotocore.mediapackagev2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [types-aiobotocore-mediapackagev2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/README.md` & `types-aiobotocore-mediapackagev2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackagev2)](https://pepy.tech/project/types-aiobotocore-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mediapackagev2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[aiobotocore.mediapackagev2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [types-aiobotocore-mediapackagev2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/setup.py` & `types-aiobotocore-mediapackagev2-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackagev2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.mediapackagev2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.mediapackagev2 2.9.1 service generated with"
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
     keywords="aiobotocore mediapackagev2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediapackagev2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/__init__.py` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListChannelGroupsPaginator,
     ListChannelsPaginator,
     ListOriginEndpointsPaginator,
 )
 
 Client = mediapackagev2Client
 
-
 __all__ = (
     "Client",
     "ListChannelGroupsPaginator",
     "ListChannelsPaginator",
     "ListOriginEndpointsPaginator",
     "mediapackagev2Client",
 )
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/__init__.pyi` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/__main__.py` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.mediapackagev2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.mediapackagev2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\nOther"
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

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/client.py` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("mediapackagev2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -113,30 +112,30 @@
     async def create_channel(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Create a channel to start receiving content streams.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#create_channel)
         """
 
     async def create_channel_group(
         self,
         *,
         ChannelGroupName: str,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateChannelGroupResponseTypeDef:
         """
         Create a channel group to group your channels and origin endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_channel_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#create_channel_group)
         """
@@ -150,15 +149,15 @@
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateOriginEndpointResponseTypeDef:
         """
         The endpoint is attached to a channel, and represents the output of the live
         content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#create_origin_endpoint)
@@ -310,15 +309,15 @@
 
     async def list_origin_endpoints(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOriginEndpointsResponseTypeDef:
         """
         Retrieves all origin endpoints in a specific channel that are configured in AWS
         Elemental
         MediaPackage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.list_origin_endpoints)
@@ -403,15 +402,15 @@
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
-        LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...
+        LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#update_origin_endpoint)
         """
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/client.pyi` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,30 +109,30 @@
     async def create_channel(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateChannelResponseTypeDef:
         """
         Create a channel to start receiving content streams.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#create_channel)
         """
 
     async def create_channel_group(
         self,
         *,
         ChannelGroupName: str,
         ClientToken: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateChannelGroupResponseTypeDef:
         """
         Create a channel group to group your channels and origin endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_channel_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#create_channel_group)
         """
@@ -146,15 +146,15 @@
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateOriginEndpointResponseTypeDef:
         """
         The endpoint is attached to a channel, and represents the output of the live
         content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.create_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#create_origin_endpoint)
@@ -306,15 +306,15 @@
 
     async def list_origin_endpoints(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListOriginEndpointsResponseTypeDef:
         """
         Retrieves all origin endpoints in a specific channel that are configured in AWS
         Elemental
         MediaPackage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.list_origin_endpoints)
@@ -399,15 +399,15 @@
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
         Segment: SegmentTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
-        LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...
+        LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Client.update_origin_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/client/#update_origin_endpoint)
         """
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/literals.py` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/literals.py`

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
     "AdMarkerHlsType",
     "CmafEncryptionMethodType",
     "ContainerTypeType",
     "DrmSystemType",
     "ListChannelGroupsPaginatorName",
     "ListChannelsPaginatorName",
@@ -35,15 +34,14 @@
     "mediapackagev2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdMarkerHlsType = Literal["DATERANGE"]
 CmafEncryptionMethodType = Literal["CBCS", "CENC"]
 ContainerTypeType = Literal["CMAF", "TS"]
 DrmSystemType = Literal["CLEAR_KEY_AES_128", "FAIRPLAY", "PLAYREADY", "WIDEVINE"]
 ListChannelGroupsPaginatorName = Literal["list_channel_groups"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListOriginEndpointsPaginatorName = Literal["list_origin_endpoints"]
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/literals.pyi` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/paginator.py` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListChannelGroupsPaginator", "ListChannelsPaginator", "ListOriginEndpointsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -87,13 +86,13 @@
     """
 
     def paginate(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/paginator.pyi` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
     """
 
     def paginate(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/type_defs.py` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2/type_defs.pyi` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/PKG-INFO` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackagev2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.mediapackagev2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.mediapackagev2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/
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
 
 <a id="types-aiobotocore-mediapackagev2"></a>
 
 # types-aiobotocore-mediapackagev2
 
 [![PyPI - types-aiobotocore-mediapackagev2](https://img.shields.io/pypi/v/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackagev2)](https://pepy.tech/project/types-aiobotocore-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mediapackagev2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[aiobotocore.mediapackagev2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [types-aiobotocore-mediapackagev2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackagev2-2.9.0/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackagev2-2.9.1/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

