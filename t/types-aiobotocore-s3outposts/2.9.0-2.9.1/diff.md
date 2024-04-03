# Comparing `tmp/types-aiobotocore-s3outposts-2.9.0.tar.gz` & `tmp/types-aiobotocore-s3outposts-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3outposts-2.9.0.tar", last modified: Wed Dec 13 20:00:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3outposts-2.9.1.tar", last modified: Thu Jan 18 01:21:42 2024, max compression
```

## Comparing `types-aiobotocore-s3outposts-2.9.0.tar` & `types-aiobotocore-s3outposts-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.425198 types-aiobotocore-s3outposts-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2023-12-13 20:00:23.425198 types-aiobotocore-s3outposts-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11905 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:23.425198 types-aiobotocore-s3outposts-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.425198 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2023-12-13 19:55:16.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2023-12-13 19:55:16.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2023-12-13 19:55:16.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2023-12-13 19:55:16.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:15.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:23.425198 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2023-12-13 20:00:23.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 20:00:23.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:23.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:23.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:23.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:23.000000 types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.457063 types-aiobotocore-s3outposts-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-01-18 01:21:42.457063 types-aiobotocore-s3outposts-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11905 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:42.457063 types-aiobotocore-s3outposts-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.453063 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-01-18 01:16:48.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-01-18 01:16:48.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-01-18 01:16:48.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-01-18 01:16:48.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-01-18 01:16:48.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-01-18 01:16:48.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:47.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:42.457063 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-01-18 01:21:42.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:21:42.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:42.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:42.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:42.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:42.000000 types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/LICENSE` & `types-aiobotocore-s3outposts-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-s3outposts-2.9.0/PKG-INFO` & `types-aiobotocore-s3outposts-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3outposts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.S3Outposts 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.S3Outposts 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/
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
 
 <a id="types-aiobotocore-s3outposts"></a>
 
 # types-aiobotocore-s3outposts
 
 [![PyPI - types-aiobotocore-s3outposts](https://img.shields.io/pypi/v/types-aiobotocore-s3outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3outposts)](https://pepy.tech/project/types-aiobotocore-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Outposts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[aiobotocore.S3Outposts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [types-aiobotocore-s3outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/README.md` & `types-aiobotocore-s3outposts-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3outposts)](https://pepy.tech/project/types-aiobotocore-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Outposts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[aiobotocore.S3Outposts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [types-aiobotocore-s3outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/setup.py` & `types-aiobotocore-s3outposts-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3outposts",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_s3outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3Outposts 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.S3Outposts 2.9.1 service generated with"
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
     keywords="aiobotocore s3outposts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_s3outposts": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/__init__.py` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListEndpointsPaginator,
     ListOutpostsWithS3Paginator,
     ListSharedEndpointsPaginator,
 )
 
 Client = S3OutpostsClient
 
-
 __all__ = (
     "Client",
     "ListEndpointsPaginator",
     "ListOutpostsWithS3Paginator",
     "ListSharedEndpointsPaginator",
     "S3OutpostsClient",
 )
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/__init__.pyi` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/__main__.py` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3Outposts 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.S3Outposts 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts\nOther"
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

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/client.py` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("S3OutpostsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -99,15 +98,15 @@
     async def create_endpoint(
         self,
         *,
         OutpostId: str,
         SubnetId: str,
         SecurityGroupId: str,
         AccessType: EndpointAccessTypeType = ...,
-        CustomerOwnedIpv4Pool: str = ...
+        CustomerOwnedIpv4Pool: str = ...,
     ) -> CreateEndpointResultTypeDef:
         """
         Creates an endpoint and associates it with the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/client/#create_endpoint)
         """
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/client.pyi` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     async def create_endpoint(
         self,
         *,
         OutpostId: str,
         SubnetId: str,
         SecurityGroupId: str,
         AccessType: EndpointAccessTypeType = ...,
-        CustomerOwnedIpv4Pool: str = ...
+        CustomerOwnedIpv4Pool: str = ...,
     ) -> CreateEndpointResultTypeDef:
         """
         Creates an endpoint and associates it with the specified Outpost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/client/#create_endpoint)
         """
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/literals.py` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "EndpointAccessTypeType",
     "EndpointStatusType",
     "ListEndpointsPaginatorName",
     "ListOutpostsWithS3PaginatorName",
     "ListSharedEndpointsPaginatorName",
     "S3OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 EndpointAccessTypeType = Literal["CustomerOwnedIp", "Private"]
 EndpointStatusType = Literal["Available", "Create_Failed", "Delete_Failed", "Deleting", "Pending"]
 ListEndpointsPaginatorName = Literal["list_endpoints"]
 ListOutpostsWithS3PaginatorName = Literal["list_outposts_with_s3"]
 ListSharedEndpointsPaginatorName = Literal["list_shared_endpoints"]
 S3OutpostsServiceName = Literal["s3outposts"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/literals.pyi` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/paginator.py` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListOutpostsWithS3ResultTypeDef,
     ListSharedEndpointsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListEndpointsPaginator", "ListOutpostsWithS3Paginator", "ListSharedEndpointsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/paginator.pyi` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/type_defs.py` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/type_defs.py`

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
     "CreateEndpointRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "FailedReasonTypeDef",
     "NetworkInterfaceTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts/type_defs.pyi` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/PKG-INFO` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3outposts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.S3Outposts 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.S3Outposts 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/
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
 
 <a id="types-aiobotocore-s3outposts"></a>
 
 # types-aiobotocore-s3outposts
 
 [![PyPI - types-aiobotocore-s3outposts](https://img.shields.io/pypi/v/types-aiobotocore-s3outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3outposts)](https://pepy.tech/project/types-aiobotocore-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Outposts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[aiobotocore.S3Outposts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
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
 [types-aiobotocore-s3outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3outposts-2.9.0/types_aiobotocore_s3outposts.egg-info/SOURCES.txt` & `types-aiobotocore-s3outposts-2.9.1/types_aiobotocore_s3outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

