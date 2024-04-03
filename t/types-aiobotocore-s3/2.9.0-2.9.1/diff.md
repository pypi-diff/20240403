# Comparing `tmp/types-aiobotocore-s3-2.9.0.tar.gz` & `tmp/types-aiobotocore-s3-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3-2.9.0.tar", last modified: Wed Dec 13 20:00:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3-2.9.1.tar", last modified: Thu Jan 18 01:21:41 2024, max compression
```

## Comparing `types-aiobotocore-s3-2.9.0.tar` & `types-aiobotocore-s3-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:22.625205 types-aiobotocore-s3-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2023-12-13 20:00:22.621205 types-aiobotocore-s3-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16356 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:22.625205 types-aiobotocore-s3-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:22.621205 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83543 2023-12-13 19:55:05.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    83539 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17775 2023-12-13 19:55:07.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    17773 2023-12-13 19:55:07.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2023-12-13 19:55:06.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2023-12-13 19:55:06.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   123684 2023-12-13 19:55:06.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   123638 2023-12-13 19:55:06.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   159447 2023-12-13 19:55:09.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   159446 2023-12-13 19:55:08.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:02.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2023-12-13 19:55:06.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2023-12-13 19:55:06.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:22.621205 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2023-12-13 20:00:22.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-13 20:00:22.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:22.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:22.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:22.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 20:00:22.000000 types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.733067 types-aiobotocore-s3-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-01-18 01:21:41.733067 types-aiobotocore-s3-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16356 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:41.733067 types-aiobotocore-s3-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.729067 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83595 2024-01-18 01:16:40.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83592 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-01-18 01:16:42.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-01-18 01:16:42.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-01-18 01:16:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-01-18 01:16:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   124521 2024-01-18 01:16:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124478 2024-01-18 01:16:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   159446 2024-01-18 01:16:45.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   159446 2024-01-18 01:16:44.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:36.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-01-18 01:16:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-01-18 01:16:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.733067 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-01-18 01:21:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-18 01:21:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 01:21:41.000000 types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3-2.9.0/LICENSE` & `types-aiobotocore-s3-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-s3-2.9.0/PKG-INFO` & `types-aiobotocore-s3-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.S3 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.S3 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/
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
 
 <a id="types-aiobotocore-s3"></a>
 
 # types-aiobotocore-s3
 
 [![PyPI - types-aiobotocore-s3](https://img.shields.io/pypi/v/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3)](https://pepy.tech/project/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
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
 [types-aiobotocore-s3 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3-2.9.0/README.md` & `types-aiobotocore-s3-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3)](https://pepy.tech/project/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
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
 [types-aiobotocore-s3 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3-2.9.0/setup.py` & `types-aiobotocore-s3-2.9.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,47 +7,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3 2.9.0 service generated with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.S3 2.9.1 service generated with mypy-boto3-builder 7.23.1"
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
     keywords="aiobotocore s3 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_s3": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/__init__.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,18 +57,16 @@
     BucketNotExistsWaiter,
     ObjectExistsWaiter,
     ObjectNotExistsWaiter,
 )
 
 Client = S3Client
 
-
 ServiceResource = S3ServiceResource
 
-
 __all__ = (
     "BucketExistsWaiter",
     "BucketNotExistsWaiter",
     "Client",
     "ListDirectoryBucketsPaginator",
     "ListMultipartUploadsPaginator",
     "ListObjectVersionsPaginator",
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/__init__.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/__main__.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.S3 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
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

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/client.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
 else:
     from typing_extensions import Literal
 try:
     from boto3.s3.transfer import TransferConfig
 except ImportError:
     from builtins import object as TransferConfig
 
-
 __all__ = ("S3Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -206,15 +205,15 @@
     async def abort_multipart_upload(
         self,
         *,
         Bucket: str,
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> AbortMultipartUploadOutputTypeDef:
         """
         This operation aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.abort_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#abort_multipart_upload)
         """
@@ -246,15 +245,15 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> CompleteMultipartUploadOutputTypeDef:
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.complete_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#complete_multipart_upload)
         """
@@ -315,15 +314,15 @@
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#copy_object)
         """
@@ -336,15 +335,15 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        ObjectOwnership: ObjectOwnershipType = ...
+        ObjectOwnership: ObjectOwnershipType = ...,
     ) -> CreateBucketOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#create_bucket)
         """
@@ -377,15 +376,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> CreateMultipartUploadOutputTypeDef:
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#create_multipart_upload)
         """
@@ -537,15 +536,15 @@
         *,
         Bucket: str,
         Key: str,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#delete_object)
         """
@@ -565,15 +564,15 @@
         *,
         Bucket: str,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> DeleteObjectsOutputTypeDef:
         """
         This operation enables you to delete multiple objects from a bucket using a
         single HTTP
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_objects)
@@ -652,15 +651,15 @@
         """
 
     async def get_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> GetBucketAccelerateConfigurationOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_accelerate_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_bucket_accelerate_configuration)
         """
@@ -894,15 +893,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object)
         """
@@ -910,15 +909,15 @@
     async def get_object_acl(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectAclOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_acl)
         """
@@ -932,15 +931,15 @@
         VersionId: str = ...,
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectAttributesOutputTypeDef:
         """
         Retrieves all the metadata from an object without returning the object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_attributes)
         """
@@ -948,15 +947,15 @@
     async def get_object_legal_hold(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectLegalHoldOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_legal_hold)
         """
@@ -974,15 +973,15 @@
     async def get_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectRetentionOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_retention)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_retention)
         """
@@ -990,30 +989,30 @@
     async def get_object_tagging(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> GetObjectTaggingOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_tagging)
         """
 
     async def get_object_torrent(
         self,
         *,
         Bucket: str,
         Key: str,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectTorrentOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_torrent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_torrent)
         """
@@ -1053,15 +1052,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` operation retrieves metadata from an object without returning the
         object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.head_object)
@@ -1135,15 +1134,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> ListMultipartUploadsOutputTypeDef:
         """
         This operation lists in-progress multipart uploads in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_multipart_uploads)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_multipart_uploads)
         """
@@ -1156,15 +1155,15 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> ListObjectVersionsOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_object_versions)
         """
@@ -1176,15 +1175,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> ListObjectsOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects)
         """
@@ -1198,15 +1197,15 @@
         MaxKeys: int = ...,
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> ListObjectsV2OutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects_v2)
         """
@@ -1219,30 +1218,30 @@
         UploadId: str,
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> ListPartsOutputTypeDef:
         """
         Lists the parts that have been uploaded for a specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_parts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_parts)
         """
 
     async def put_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         AccelerateConfiguration: AccelerateConfigurationTypeDef,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_accelerate_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_accelerate_configuration)
         """
@@ -1255,45 +1254,45 @@
         AccessControlPolicy: AccessControlPolicyTypeDef = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_acl)
         """
 
     async def put_bucket_analytics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
         AnalyticsConfiguration: AnalyticsConfigurationTypeDef,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_analytics_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_analytics_configuration)
         """
 
     async def put_bucket_cors(
         self,
         *,
         Bucket: str,
         CORSConfiguration: CORSConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_cors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_cors)
         """
@@ -1301,149 +1300,149 @@
     async def put_bucket_encryption(
         self,
         *,
         Bucket: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_encryption)
         """
 
     async def put_bucket_intelligent_tiering_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef
+        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_intelligent_tiering_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_intelligent_tiering_configuration)
         """
 
     async def put_bucket_inventory_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
         InventoryConfiguration: InventoryConfigurationTypeDef,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_inventory_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_inventory_configuration)
         """
 
     async def put_bucket_lifecycle(
         self,
         *,
         Bucket: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_lifecycle)
         """
 
     async def put_bucket_lifecycle_configuration(
         self,
         *,
         Bucket: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_lifecycle_configuration)
         """
 
     async def put_bucket_logging(
         self,
         *,
         Bucket: str,
         BucketLoggingStatus: BucketLoggingStatusTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_logging)
         """
 
     async def put_bucket_metrics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
         MetricsConfiguration: MetricsConfigurationTypeDef,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_metrics_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_metrics_configuration)
         """
 
     async def put_bucket_notification(
         self,
         *,
         Bucket: str,
         NotificationConfiguration: NotificationConfigurationDeprecatedTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_notification)
         """
 
     async def put_bucket_notification_configuration(
         self,
         *,
         Bucket: str,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ExpectedBucketOwner: str = ...,
-        SkipDestinationValidation: bool = ...
+        SkipDestinationValidation: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_notification_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_notification_configuration)
         """
 
     async def put_bucket_ownership_controls(
         self,
         *,
         Bucket: str,
         OwnershipControls: OwnershipControlsTypeDef,
         ContentMD5: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_ownership_controls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_ownership_controls)
         """
@@ -1451,15 +1450,15 @@
     async def put_bucket_policy(
         self,
         *,
         Bucket: str,
         Policy: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ConfirmRemoveSelfBucketAccess: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Applies an Amazon S3 bucket policy to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_policy)
         """
@@ -1467,45 +1466,45 @@
     async def put_bucket_replication(
         self,
         *,
         Bucket: str,
         ReplicationConfiguration: ReplicationConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         Token: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_replication)
         """
 
     async def put_bucket_request_payment(
         self,
         *,
         Bucket: str,
         RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_request_payment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_request_payment)
         """
 
     async def put_bucket_tagging(
         self,
         *,
         Bucket: str,
         Tagging: TaggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_tagging)
         """
@@ -1513,30 +1512,30 @@
     async def put_bucket_versioning(
         self,
         *,
         Bucket: str,
         VersioningConfiguration: VersioningConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_versioning)
         """
 
     async def put_bucket_website(
         self,
         *,
         Bucket: str,
         WebsiteConfiguration: WebsiteConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_website)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_website)
         """
@@ -1576,15 +1575,15 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object)
         """
@@ -1600,15 +1599,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectAclOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_acl)
         """
@@ -1619,15 +1618,15 @@
         Bucket: str,
         Key: str,
         LegalHold: ObjectLockLegalHoldTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectLegalHoldOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_legal_hold)
         """
@@ -1637,15 +1636,15 @@
         *,
         Bucket: str,
         ObjectLockConfiguration: ObjectLockConfigurationTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         Token: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectLockConfigurationOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_lock_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_lock_configuration)
         """
@@ -1657,15 +1656,15 @@
         Key: str,
         Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectRetentionOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_retention)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_retention)
         """
@@ -1676,15 +1675,15 @@
         Bucket: str,
         Key: str,
         Tagging: TaggingTypeDef,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> PutObjectTaggingOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_tagging)
         """
@@ -1692,15 +1691,15 @@
     async def put_public_access_block(
         self,
         *,
         Bucket: str,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_public_access_block)
         """
@@ -1710,15 +1709,15 @@
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> RestoreObjectOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.restore_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#restore_object)
         """
@@ -1733,15 +1732,15 @@
         InputSerialization: InputSerializationTypeDef,
         OutputSerialization: OutputSerializationTypeDef,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestProgress: RequestProgressTypeDef = ...,
         ScanRange: ScanRangeTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> SelectObjectContentOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.select_object_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#select_object_content)
         """
@@ -1793,15 +1792,15 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#upload_part)
         """
@@ -1823,15 +1822,15 @@
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part_copy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#upload_part_copy)
         """
@@ -1874,15 +1873,15 @@
         ServerSideEncryption: ServerSideEncryptionType = ...,
         SSECustomerAlgorithm: str = ...,
         SSEKMSKeyId: str = ...,
         SSECustomerKeyMD5: str = ...,
         StorageClass: StorageClassType = ...,
         TagCount: int = ...,
         VersionId: str = ...,
-        BucketKeyEnabled: bool = ...
+        BucketKeyEnabled: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.write_get_object_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#write_get_object_response)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/client.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     async def abort_multipart_upload(
         self,
         *,
         Bucket: str,
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> AbortMultipartUploadOutputTypeDef:
         """
         This operation aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.abort_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#abort_multipart_upload)
         """
@@ -242,15 +242,15 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> CompleteMultipartUploadOutputTypeDef:
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.complete_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#complete_multipart_upload)
         """
@@ -311,15 +311,15 @@
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#copy_object)
         """
@@ -332,15 +332,15 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        ObjectOwnership: ObjectOwnershipType = ...
+        ObjectOwnership: ObjectOwnershipType = ...,
     ) -> CreateBucketOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#create_bucket)
         """
@@ -373,15 +373,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> CreateMultipartUploadOutputTypeDef:
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#create_multipart_upload)
         """
@@ -533,15 +533,15 @@
         *,
         Bucket: str,
         Key: str,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#delete_object)
         """
@@ -561,15 +561,15 @@
         *,
         Bucket: str,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> DeleteObjectsOutputTypeDef:
         """
         This operation enables you to delete multiple objects from a bucket using a
         single HTTP
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_objects)
@@ -648,15 +648,15 @@
         """
 
     async def get_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> GetBucketAccelerateConfigurationOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_accelerate_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_bucket_accelerate_configuration)
         """
@@ -890,15 +890,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object)
         """
@@ -906,15 +906,15 @@
     async def get_object_acl(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectAclOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_acl)
         """
@@ -928,15 +928,15 @@
         VersionId: str = ...,
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectAttributesOutputTypeDef:
         """
         Retrieves all the metadata from an object without returning the object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_attributes)
         """
@@ -944,15 +944,15 @@
     async def get_object_legal_hold(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectLegalHoldOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_legal_hold)
         """
@@ -970,15 +970,15 @@
     async def get_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectRetentionOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_retention)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_retention)
         """
@@ -986,30 +986,30 @@
     async def get_object_tagging(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> GetObjectTaggingOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_tagging)
         """
 
     async def get_object_torrent(
         self,
         *,
         Bucket: str,
         Key: str,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> GetObjectTorrentOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_torrent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#get_object_torrent)
         """
@@ -1049,15 +1049,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` operation retrieves metadata from an object without returning the
         object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.head_object)
@@ -1131,15 +1131,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> ListMultipartUploadsOutputTypeDef:
         """
         This operation lists in-progress multipart uploads in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_multipart_uploads)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_multipart_uploads)
         """
@@ -1152,15 +1152,15 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> ListObjectVersionsOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_object_versions)
         """
@@ -1172,15 +1172,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> ListObjectsOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects)
         """
@@ -1194,15 +1194,15 @@
         MaxKeys: int = ...,
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> ListObjectsV2OutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects_v2)
         """
@@ -1215,30 +1215,30 @@
         UploadId: str,
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> ListPartsOutputTypeDef:
         """
         Lists the parts that have been uploaded for a specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_parts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_parts)
         """
 
     async def put_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         AccelerateConfiguration: AccelerateConfigurationTypeDef,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_accelerate_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_accelerate_configuration)
         """
@@ -1251,45 +1251,45 @@
         AccessControlPolicy: AccessControlPolicyTypeDef = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_acl)
         """
 
     async def put_bucket_analytics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
         AnalyticsConfiguration: AnalyticsConfigurationTypeDef,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_analytics_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_analytics_configuration)
         """
 
     async def put_bucket_cors(
         self,
         *,
         Bucket: str,
         CORSConfiguration: CORSConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_cors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_cors)
         """
@@ -1297,149 +1297,149 @@
     async def put_bucket_encryption(
         self,
         *,
         Bucket: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_encryption)
         """
 
     async def put_bucket_intelligent_tiering_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef
+        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_intelligent_tiering_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_intelligent_tiering_configuration)
         """
 
     async def put_bucket_inventory_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
         InventoryConfiguration: InventoryConfigurationTypeDef,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_inventory_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_inventory_configuration)
         """
 
     async def put_bucket_lifecycle(
         self,
         *,
         Bucket: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_lifecycle)
         """
 
     async def put_bucket_lifecycle_configuration(
         self,
         *,
         Bucket: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_lifecycle_configuration)
         """
 
     async def put_bucket_logging(
         self,
         *,
         Bucket: str,
         BucketLoggingStatus: BucketLoggingStatusTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_logging)
         """
 
     async def put_bucket_metrics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
         MetricsConfiguration: MetricsConfigurationTypeDef,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_metrics_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_metrics_configuration)
         """
 
     async def put_bucket_notification(
         self,
         *,
         Bucket: str,
         NotificationConfiguration: NotificationConfigurationDeprecatedTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_notification)
         """
 
     async def put_bucket_notification_configuration(
         self,
         *,
         Bucket: str,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ExpectedBucketOwner: str = ...,
-        SkipDestinationValidation: bool = ...
+        SkipDestinationValidation: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_notification_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_notification_configuration)
         """
 
     async def put_bucket_ownership_controls(
         self,
         *,
         Bucket: str,
         OwnershipControls: OwnershipControlsTypeDef,
         ContentMD5: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_ownership_controls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_ownership_controls)
         """
@@ -1447,15 +1447,15 @@
     async def put_bucket_policy(
         self,
         *,
         Bucket: str,
         Policy: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ConfirmRemoveSelfBucketAccess: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Applies an Amazon S3 bucket policy to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_policy)
         """
@@ -1463,45 +1463,45 @@
     async def put_bucket_replication(
         self,
         *,
         Bucket: str,
         ReplicationConfiguration: ReplicationConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         Token: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_replication)
         """
 
     async def put_bucket_request_payment(
         self,
         *,
         Bucket: str,
         RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_request_payment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_request_payment)
         """
 
     async def put_bucket_tagging(
         self,
         *,
         Bucket: str,
         Tagging: TaggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_tagging)
         """
@@ -1509,30 +1509,30 @@
     async def put_bucket_versioning(
         self,
         *,
         Bucket: str,
         VersioningConfiguration: VersioningConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_versioning)
         """
 
     async def put_bucket_website(
         self,
         *,
         Bucket: str,
         WebsiteConfiguration: WebsiteConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_website)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_website)
         """
@@ -1572,15 +1572,15 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object)
         """
@@ -1596,15 +1596,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectAclOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_acl)
         """
@@ -1615,15 +1615,15 @@
         Bucket: str,
         Key: str,
         LegalHold: ObjectLockLegalHoldTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectLegalHoldOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_legal_hold)
         """
@@ -1633,15 +1633,15 @@
         *,
         Bucket: str,
         ObjectLockConfiguration: ObjectLockConfigurationTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         Token: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectLockConfigurationOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_lock_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_lock_configuration)
         """
@@ -1653,15 +1653,15 @@
         Key: str,
         Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectRetentionOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_retention)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_retention)
         """
@@ -1672,15 +1672,15 @@
         Bucket: str,
         Key: str,
         Tagging: TaggingTypeDef,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> PutObjectTaggingOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_tagging)
         """
@@ -1688,15 +1688,15 @@
     async def put_public_access_block(
         self,
         *,
         Bucket: str,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_public_access_block)
         """
@@ -1706,15 +1706,15 @@
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> RestoreObjectOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.restore_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#restore_object)
         """
@@ -1729,15 +1729,15 @@
         InputSerialization: InputSerializationTypeDef,
         OutputSerialization: OutputSerializationTypeDef,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestProgress: RequestProgressTypeDef = ...,
         ScanRange: ScanRangeTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> SelectObjectContentOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.select_object_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#select_object_content)
         """
@@ -1789,15 +1789,15 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#upload_part)
         """
@@ -1819,15 +1819,15 @@
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part_copy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#upload_part_copy)
         """
@@ -1870,15 +1870,15 @@
         ServerSideEncryption: ServerSideEncryptionType = ...,
         SSECustomerAlgorithm: str = ...,
         SSEKMSKeyId: str = ...,
         SSECustomerKeyMD5: str = ...,
         StorageClass: StorageClassType = ...,
         TagCount: int = ...,
         VersionId: str = ...,
-        BucketKeyEnabled: bool = ...
+        BucketKeyEnabled: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.write_get_object_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#write_get_object_response)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/literals.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/literals.py`

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
     "AnalyticsS3ExportFileFormatType",
     "ArchiveStatusType",
     "BucketAccelerateStatusType",
     "BucketCannedACLType",
     "BucketExistsWaiterName",
     "BucketLocationConstraintType",
@@ -99,15 +98,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AnalyticsS3ExportFileFormatType = Literal["CSV"]
 ArchiveStatusType = Literal["ARCHIVE_ACCESS", "DEEP_ARCHIVE_ACCESS"]
 BucketAccelerateStatusType = Literal["Enabled", "Suspended"]
 BucketCannedACLType = Literal["authenticated-read", "private", "public-read", "public-read-write"]
 BucketExistsWaiterName = Literal["bucket_exists"]
 BucketLocationConstraintType = Literal[
     "EU",
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/literals.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/paginator.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDirectoryBucketsPaginator",
     "ListMultipartUploadsPaginator",
     "ListObjectVersionsPaginator",
     "ListObjectsPaginator",
     "ListObjectsV2Paginator",
     "ListPartsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -99,15 +97,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listmultipartuploadspaginator)
         """
 
 
@@ -123,15 +121,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectversionspaginator)
         """
 
 
@@ -147,15 +145,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectspaginator)
         """
 
 
@@ -173,15 +171,15 @@
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectsv2paginator)
         """
 
 
@@ -198,13 +196,13 @@
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listpartspaginator)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/paginator.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listmultipartuploadspaginator)
         """
 
 class ListObjectVersionsPaginator(AioPaginator):
@@ -117,15 +117,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectversionspaginator)
         """
 
 class ListObjectsPaginator(AioPaginator):
@@ -140,15 +140,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectspaginator)
         """
 
 class ListObjectsV2Paginator(AioPaginator):
@@ -165,15 +165,15 @@
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectsv2paginator)
         """
 
 class ListPartsPaginator(AioPaginator):
@@ -189,13 +189,13 @@
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listpartspaginator)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/service_resource.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 except ImportError:
     from builtins import object as ResourceMeta
 try:
     from boto3.s3.transfer import TransferConfig
 except ImportError:
     from builtins import object as TransferConfig
 
-
 __all__ = (
     "S3ServiceResource",
     "Bucket",
     "BucketAcl",
     "BucketCors",
     "BucketLifecycle",
     "BucketLifecycleConfiguration",
@@ -169,15 +168,14 @@
     "ServiceResourceBucketsCollection",
     "BucketMultipartUploadsCollection",
     "BucketObjectVersionsCollection",
     "BucketObjectsCollection",
     "MultipartUploadPartsCollection",
 )
 
-
 class ServiceResourceBucketsCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.buckets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#serviceresourcebucketscollection)
     """
 
     def all(self) -> "ServiceResourceBucketsCollection":
@@ -232,15 +230,14 @@
         """
         A generator which yields Buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.buckets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#serviceresourcebucketscollection)
         """
 
-
 class BucketMultipartUploadsCollection(AIOResourceCollection):
     def all(self) -> "BucketMultipartUploadsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -249,15 +246,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> "BucketMultipartUploadsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "BucketMultipartUploadsCollection":
         """
@@ -280,15 +277,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUpload"]:
         """
         A generator which yields MultipartUploads.
         """
 
-
 class BucketObjectVersionsCollection(AIOResourceCollection):
     def all(self) -> "BucketObjectVersionsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -298,28 +294,28 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> "BucketObjectVersionsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectVersionsCollection":
         """
@@ -342,15 +338,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["ObjectVersion"]:
         """
         A generator which yields ObjectVersions.
         """
 
-
 class BucketObjectsCollection(AIOResourceCollection):
     def all(self) -> "BucketObjectsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -359,28 +354,28 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> "BucketObjectsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectsCollection":
         """
@@ -403,15 +398,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["ObjectSummary"]:
         """
         A generator which yields ObjectSummarys.
         """
 
-
 class MultipartUploadPartsCollection(AIOResourceCollection):
     def all(self) -> "MultipartUploadPartsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -419,15 +413,15 @@
         *,
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> "MultipartUploadPartsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "MultipartUploadPartsCollection":
         """
@@ -450,24 +444,24 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUploadPart"]:
         """
         A generator which yields MultipartUploadParts.
         """
 
-
 class BucketAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketacl)
     """
 
     owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketaclbucket-method)
@@ -498,15 +492,15 @@
         AccessControlPolicy: AccessControlPolicyTypeDef = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketaclput-method)
         """
@@ -517,26 +511,25 @@
         BucketAcl
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketaclreload-method)
         """
 
-
 _BucketAcl = BucketAcl
 
-
 class BucketCors(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcors)
     """
 
     cors_rules: Awaitable[List[CORSRuleBucketCorsTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsbucket-method)
@@ -569,15 +562,15 @@
         """
 
     async def put(
         self,
         *,
         CORSConfiguration: CORSConfigurationBucketCorsTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsput-method)
         """
@@ -588,26 +581,25 @@
         BucketCors
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsreload-method)
         """
 
-
 _BucketCors = BucketCors
 
-
 class BucketLifecycle(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycle)
     """
 
     rules: Awaitable[List[RuleBucketLifecycleTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecyclebucket-method)
@@ -640,15 +632,15 @@
         """
 
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: LifecycleConfigurationBucketLifecycleTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleput-method)
         """
@@ -659,26 +651,25 @@
         BucketLifecycle
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecyclereload-method)
         """
 
-
 _BucketLifecycle = BucketLifecycle
 
-
 class BucketLifecycleConfiguration(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
     rules: Awaitable[List[LifecycleRuleBucketLifecycleConfigurationTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationbucket-method)
@@ -711,15 +702,15 @@
         """
 
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationput-method)
         """
@@ -730,26 +721,25 @@
         attributes of the BucketLifecycleConfiguration
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationreload-method)
         """
 
-
 _BucketLifecycleConfiguration = BucketLifecycleConfiguration
 
-
 class BucketLogging(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLogging)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlogging)
     """
 
     logging_enabled: Awaitable[LoggingEnabledResponseTypeDef]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingbucket-method)
@@ -774,15 +764,15 @@
         """
 
     async def put(
         self,
         *,
         BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingput-method)
         """
@@ -793,31 +783,30 @@
         BucketLogging
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingreload-method)
         """
 
-
 _BucketLogging = BucketLogging
 
-
 class BucketNotification(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotification)
     """
 
     topic_configurations: Awaitable[List[TopicConfigurationBucketNotificationTypeDef]]
     queue_configurations: Awaitable[List[QueueConfigurationBucketNotificationTypeDef]]
     lambda_function_configurations: Awaitable[
         List[LambdaFunctionConfigurationBucketNotificationTypeDef]
     ]
     event_bridge_configuration: Awaitable[Dict[str, Any]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationbucket-method)
@@ -842,15 +831,15 @@
         """
 
     async def put(
         self,
         *,
         NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,
         ExpectedBucketOwner: str = ...,
-        SkipDestinationValidation: bool = ...
+        SkipDestinationValidation: bool = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationput-method)
         """
@@ -861,26 +850,25 @@
         attributes of the BucketNotification
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationreload-method)
         """
 
-
 _BucketNotification = BucketNotification
 
-
 class BucketPolicy(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketPolicy)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicy)
     """
 
     policy: Awaitable[str]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketPolicy.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicybucket-method)
@@ -914,15 +902,15 @@
 
     async def put(
         self,
         *,
         Policy: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ConfirmRemoveSelfBucketAccess: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         Applies an Amazon S3 bucket policy to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketPolicy.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicyput-method)
         """
@@ -933,26 +921,25 @@
         BucketPolicy
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketPolicy.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicyreload-method)
         """
 
-
 _BucketPolicy = BucketPolicy
 
-
 class BucketRequestPayment(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketRequestPayment)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpayment)
     """
 
     payer: Awaitable[PayerType]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketRequestPayment.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpaymentbucket-method)
@@ -977,15 +964,15 @@
         """
 
     async def put(
         self,
         *,
         RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketRequestPayment.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpaymentput-method)
         """
@@ -996,26 +983,25 @@
         of the BucketRequestPayment
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketRequestPayment.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpaymentreload-method)
         """
 
-
 _BucketRequestPayment = BucketRequestPayment
 
-
 class BucketTagging(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketTagging)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettagging)
     """
 
     tag_set: Awaitable[List[TagTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettaggingbucket-method)
@@ -1048,15 +1034,15 @@
         """
 
     async def put(
         self,
         *,
         Tagging: TaggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettaggingput-method)
         """
@@ -1067,42 +1053,41 @@
         BucketTagging
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettaggingreload-method)
         """
 
-
 _BucketTagging = BucketTagging
 
-
 class BucketVersioning(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketVersioning)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioning)
     """
 
     status: Awaitable[BucketVersioningStatusType]
     mfa_delete: Awaitable[MFADeleteStatusType]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningbucket-method)
         """
 
     async def enable(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.enable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningenable-method)
         """
@@ -1127,15 +1112,15 @@
 
     async def put(
         self,
         *,
         VersioningConfiguration: VersioningConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningput-method)
         """
@@ -1151,38 +1136,37 @@
         """
 
     async def suspend(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.suspend)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningsuspend-method)
         """
 
-
 _BucketVersioning = BucketVersioning
 
-
 class BucketWebsite(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketWebsite)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsite)
     """
 
     redirect_all_requests_to: Awaitable[RedirectAllRequestsToResponseTypeDef]
     index_document: Awaitable[IndexDocumentResponseTypeDef]
     error_document: Awaitable[ErrorDocumentResponseTypeDef]
     routing_rules: Awaitable[List[RoutingRuleTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsitebucket-method)
@@ -1215,15 +1199,15 @@
         """
 
     async def put(
         self,
         *,
         WebsiteConfiguration: WebsiteConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsiteput-method)
         """
@@ -1234,18 +1218,16 @@
         BucketWebsite
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsitereload-method)
         """
 
-
 _BucketWebsite = BucketWebsite
 
-
 class MultipartUploadPart(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUploadPart)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpart)
     """
 
     last_modified: Awaitable[datetime]
@@ -1255,14 +1237,15 @@
     checksum_crc32_c: Awaitable[str]
     checksum_sha1: Awaitable[str]
     checksum_sha256: Awaitable[str]
     bucket_name: str
     object_key: str
     multipart_upload_id: str
     part_number: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def MultipartUpload(self) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpartmultipartupload-method)
@@ -1281,15 +1264,15 @@
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.copy_from)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpartcopy_from-method)
         """
@@ -1313,38 +1296,37 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpartupload-method)
         """
 
-
 _MultipartUploadPart = MultipartUploadPart
 
-
 class ObjectAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectacl)
     """
 
     owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     request_charged: Awaitable[Literal["requester"]]
     bucket_name: str
     object_key: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectaclobject-method)
@@ -1377,15 +1359,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectAclOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectaclput-method)
         """
@@ -1396,18 +1378,16 @@
         ObjectAcl
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectaclreload-method)
         """
 
-
 _ObjectAcl = ObjectAcl
 
-
 class ObjectVersion(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectVersion)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversion)
     """
 
     e_tag: Awaitable[str]
@@ -1419,14 +1399,15 @@
     is_latest: Awaitable[bool]
     last_modified: Awaitable[datetime]
     owner: Awaitable[OwnerResponseTypeDef]
     restore_status: Awaitable[RestoreStatusResponseTypeDef]
     bucket_name: str
     object_key: str
     id: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversionobject-method)
@@ -1434,15 +1415,15 @@
 
     async def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversiondelete-method)
         """
@@ -1463,15 +1444,15 @@
         ResponseExpires: TimestampTypeDef = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.get)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversionget-method)
         """
@@ -1494,29 +1475,27 @@
         Range: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` operation retrieves metadata from an object without returning the
         object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.head)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversionhead-method)
         """
 
-
 _ObjectVersion = ObjectVersion
 
-
 class MultipartUpload(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUpload)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartupload)
     """
 
     upload_id: Awaitable[str]
@@ -1526,24 +1505,25 @@
     owner: Awaitable[OwnerTypeDef]
     initiator: Awaitable[InitiatorResponseTypeDef]
     checksum_algorithm: Awaitable[ChecksumAlgorithmType]
     bucket_name: str
     object_key: str
     id: str
     parts: MultipartUploadPartsCollection
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadobject-method)
         """
 
-    async def Part(self, part_number: str) -> _MultipartUploadPart:
+    async def Part(self, part_number: str) -> "_MultipartUploadPart":
         """
         Creates a MultipartUploadPart resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpart-method)
         """
 
@@ -1565,15 +1545,15 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> "_Object":
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.complete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadcomplete-method)
         """
@@ -1582,18 +1562,16 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadget_available_subresources-method)
         """
 
-
 _MultipartUpload = MultipartUpload
 
-
 class Object(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Object)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#object)
     """
 
     delete_marker: Awaitable[bool]
@@ -1628,16 +1606,17 @@
     replication_status: Awaitable[ReplicationStatusType]
     parts_count: Awaitable[int]
     object_lock_mode: Awaitable[ObjectLockModeType]
     object_lock_retain_until_date: Awaitable[datetime]
     object_lock_legal_hold_status: Awaitable[ObjectLockLegalHoldStatusType]
     bucket_name: str
     key: str
+    meta: Awaitable["S3ResourceMeta"]
 
-    async def Acl(self) -> _ObjectAcl:
+    async def Acl(self) -> "_ObjectAcl":
         """
         Creates a ObjectAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.Acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectacl-method)
         """
 
@@ -1645,23 +1624,23 @@
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectbucket-method)
         """
 
-    async def MultipartUpload(self, id: str) -> _MultipartUpload:
+    async def MultipartUpload(self, id: str) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectmultipartupload-method)
         """
 
-    async def Version(self, id: str) -> _ObjectVersion:
+    async def Version(self, id: str) -> "_ObjectVersion":
         """
         Creates a ObjectVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.Version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversion-method)
         """
 
@@ -1717,15 +1696,15 @@
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.copy_from)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectcopy_from-method)
         """
@@ -1733,15 +1712,15 @@
     async def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectdelete-method)
         """
@@ -1791,15 +1770,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.get)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectget-method)
         """
@@ -1838,16 +1817,16 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> _MultipartUpload:
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
+    ) -> "_MultipartUpload":
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectinitiate_multipart_upload-method)
         """
 
@@ -1893,15 +1872,15 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectput-method)
         """
@@ -1918,15 +1897,15 @@
     async def restore_object(
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> RestoreObjectOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.restore_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectrestore_object-method)
         """
@@ -1971,18 +1950,16 @@
         """
         Waits until this Object is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.wait_until_not_exists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectwait_until_not_exists-method)
         """
 
-
 _Object = Object
 
-
 class ObjectSummary(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectSummary)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummary)
     """
 
     last_modified: Awaitable[datetime]
@@ -1990,16 +1967,17 @@
     checksum_algorithm: Awaitable[List[ChecksumAlgorithmType]]
     size: Awaitable[int]
     storage_class: Awaitable[ObjectStorageClassType]
     owner: Awaitable[OwnerTypeDef]
     restore_status: Awaitable[RestoreStatusTypeDef]
     bucket_name: str
     key: str
+    meta: Awaitable["S3ResourceMeta"]
 
-    async def Acl(self) -> _ObjectAcl:
+    async def Acl(self) -> "_ObjectAcl":
         """
         Creates a ObjectAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryacl-method)
         """
 
@@ -2007,31 +1985,31 @@
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarybucket-method)
         """
 
-    async def MultipartUpload(self, id: str) -> _MultipartUpload:
+    async def MultipartUpload(self, id: str) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarymultipartupload-method)
         """
 
-    async def Object(self) -> _Object:
+    async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryobject-method)
         """
 
-    async def Version(self, id: str) -> _ObjectVersion:
+    async def Version(self, id: str) -> "_ObjectVersion":
         """
         Creates a ObjectVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryversion-method)
         """
 
@@ -2072,15 +2050,15 @@
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.copy_from)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarycopy_from-method)
         """
@@ -2088,15 +2066,15 @@
     async def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarydelete-method)
         """
@@ -2118,15 +2096,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.get)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryget-method)
         """
@@ -2165,16 +2143,16 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> _MultipartUpload:
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
+    ) -> "_MultipartUpload":
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryinitiate_multipart_upload-method)
         """
 
@@ -2220,15 +2198,15 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryput-method)
         """
@@ -2236,15 +2214,15 @@
     async def restore_object(
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> RestoreObjectOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.restore_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryrestore_object-method)
         """
@@ -2261,119 +2239,118 @@
         """
         Waits until this ObjectSummary is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.wait_until_not_exists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarywait_until_not_exists-method)
         """
 
-
 _ObjectSummary = ObjectSummary
 
-
 class Bucket(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Bucket)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucket)
     """
 
     creation_date: Awaitable[datetime]
     name: str
     multipart_uploads: BucketMultipartUploadsCollection
     object_versions: BucketObjectVersionsCollection
     objects: BucketObjectsCollection
+    meta: Awaitable["S3ResourceMeta"]
 
-    async def Acl(self) -> _BucketAcl:
+    async def Acl(self) -> "_BucketAcl":
         """
         Creates a BucketAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketacl-method)
         """
 
-    async def Cors(self) -> _BucketCors:
+    async def Cors(self) -> "_BucketCors":
         """
         Creates a BucketCors resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Cors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcors-method)
         """
 
-    async def Lifecycle(self) -> _BucketLifecycle:
+    async def Lifecycle(self) -> "_BucketLifecycle":
         """
         Creates a BucketLifecycle resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycle-method)
         """
 
-    async def LifecycleConfiguration(self) -> _BucketLifecycleConfiguration:
+    async def LifecycleConfiguration(self) -> "_BucketLifecycleConfiguration":
         """
         Creates a BucketLifecycleConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.LifecycleConfiguration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfiguration-method)
         """
 
-    async def Logging(self) -> _BucketLogging:
+    async def Logging(self) -> "_BucketLogging":
         """
         Creates a BucketLogging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlogging-method)
         """
 
-    async def Notification(self) -> _BucketNotification:
+    async def Notification(self) -> "_BucketNotification":
         """
         Creates a BucketNotification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotification-method)
         """
 
-    async def Object(self, key: str) -> _Object:
+    async def Object(self, key: str) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketobject-method)
         """
 
-    async def Policy(self) -> _BucketPolicy:
+    async def Policy(self) -> "_BucketPolicy":
         """
         Creates a BucketPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicy-method)
         """
 
-    async def RequestPayment(self) -> _BucketRequestPayment:
+    async def RequestPayment(self) -> "_BucketRequestPayment":
         """
         Creates a BucketRequestPayment resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.RequestPayment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpayment-method)
         """
 
-    async def Tagging(self) -> _BucketTagging:
+    async def Tagging(self) -> "_BucketTagging":
         """
         Creates a BucketTagging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettagging-method)
         """
 
-    async def Versioning(self) -> _BucketVersioning:
+    async def Versioning(self) -> "_BucketVersioning":
         """
         Creates a BucketVersioning resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioning-method)
         """
 
-    async def Website(self) -> _BucketWebsite:
+    async def Website(self) -> "_BucketWebsite":
         """
         Creates a BucketWebsite resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Website)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsite-method)
         """
 
@@ -2400,15 +2377,15 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        ObjectOwnership: ObjectOwnershipType = ...
+        ObjectOwnership: ObjectOwnershipType = ...,
     ) -> CreateBucketOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.create)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcreate-method)
         """
@@ -2425,15 +2402,15 @@
         self,
         *,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> DeleteObjectsOutputTypeDef:
         """
         This operation enables you to delete multiple objects from a bucket using a
         single HTTP
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.delete_objects)
@@ -2520,16 +2497,16 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
-    ) -> _Object:
+        ExpectedBucketOwner: str = ...,
+    ) -> "_Object":
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketput_object-method)
         """
 
@@ -2575,170 +2552,171 @@
         """
         Waits until this Bucket is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.wait_until_not_exists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwait_until_not_exists-method)
         """
 
-
 _Bucket = Bucket
 
-
 class S3ResourceMeta(ResourceMeta):
     client: S3Client
 
-
 class S3ServiceResource(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/)
     """
 
     meta: "S3ResourceMeta"
     buckets: ServiceResourceBucketsCollection
 
-    async def Bucket(self, name: str) -> _Bucket:
+    async def Bucket(self, name: str) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucket-method)
         """
 
-    async def BucketAcl(self, bucket_name: str) -> _BucketAcl:
+    async def BucketAcl(self, bucket_name: str) -> "_BucketAcl":
         """
         Creates a BucketAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketacl-method)
         """
 
-    async def BucketCors(self, bucket_name: str) -> _BucketCors:
+    async def BucketCors(self, bucket_name: str) -> "_BucketCors":
         """
         Creates a BucketCors resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketcors-method)
         """
 
-    async def BucketLifecycle(self, bucket_name: str) -> _BucketLifecycle:
+    async def BucketLifecycle(self, bucket_name: str) -> "_BucketLifecycle":
         """
         Creates a BucketLifecycle resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketlifecycle-method)
         """
 
-    async def BucketLifecycleConfiguration(self, bucket_name: str) -> _BucketLifecycleConfiguration:
+    async def BucketLifecycleConfiguration(
+        self, bucket_name: str
+    ) -> "_BucketLifecycleConfiguration":
         """
         Creates a BucketLifecycleConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketlifecycleconfiguration-method)
         """
 
-    async def BucketLogging(self, bucket_name: str) -> _BucketLogging:
+    async def BucketLogging(self, bucket_name: str) -> "_BucketLogging":
         """
         Creates a BucketLogging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLogging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketlogging-method)
         """
 
-    async def BucketNotification(self, bucket_name: str) -> _BucketNotification:
+    async def BucketNotification(self, bucket_name: str) -> "_BucketNotification":
         """
         Creates a BucketNotification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketnotification-method)
         """
 
-    async def BucketPolicy(self, bucket_name: str) -> _BucketPolicy:
+    async def BucketPolicy(self, bucket_name: str) -> "_BucketPolicy":
         """
         Creates a BucketPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketpolicy-method)
         """
 
-    async def BucketRequestPayment(self, bucket_name: str) -> _BucketRequestPayment:
+    async def BucketRequestPayment(self, bucket_name: str) -> "_BucketRequestPayment":
         """
         Creates a BucketRequestPayment resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketRequestPayment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketrequestpayment-method)
         """
 
-    async def BucketTagging(self, bucket_name: str) -> _BucketTagging:
+    async def BucketTagging(self, bucket_name: str) -> "_BucketTagging":
         """
         Creates a BucketTagging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketTagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebuckettagging-method)
         """
 
-    async def BucketVersioning(self, bucket_name: str) -> _BucketVersioning:
+    async def BucketVersioning(self, bucket_name: str) -> "_BucketVersioning":
         """
         Creates a BucketVersioning resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketVersioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketversioning-method)
         """
 
-    async def BucketWebsite(self, bucket_name: str) -> _BucketWebsite:
+    async def BucketWebsite(self, bucket_name: str) -> "_BucketWebsite":
         """
         Creates a BucketWebsite resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketWebsite)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketwebsite-method)
         """
 
-    async def MultipartUpload(self, bucket_name: str, object_key: str, id: str) -> _MultipartUpload:
+    async def MultipartUpload(
+        self, bucket_name: str, object_key: str, id: str
+    ) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcemultipartupload-method)
         """
 
     async def MultipartUploadPart(
         self, bucket_name: str, object_key: str, multipart_upload_id: str, part_number: str
-    ) -> _MultipartUploadPart:
+    ) -> "_MultipartUploadPart":
         """
         Creates a MultipartUploadPart resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUploadPart)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcemultipartuploadpart-method)
         """
 
-    async def Object(self, bucket_name: str, key: str) -> _Object:
+    async def Object(self, bucket_name: str, key: str) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobject-method)
         """
 
-    async def ObjectAcl(self, bucket_name: str, object_key: str) -> _ObjectAcl:
+    async def ObjectAcl(self, bucket_name: str, object_key: str) -> "_ObjectAcl":
         """
         Creates a ObjectAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobjectacl-method)
         """
 
-    async def ObjectSummary(self, bucket_name: str, key: str) -> _ObjectSummary:
+    async def ObjectSummary(self, bucket_name: str, key: str) -> "_ObjectSummary":
         """
         Creates a ObjectSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobjectsummary-method)
         """
 
-    async def ObjectVersion(self, bucket_name: str, object_key: str, id: str) -> _ObjectVersion:
+    async def ObjectVersion(self, bucket_name: str, object_key: str, id: str) -> "_ObjectVersion":
         """
         Creates a ObjectVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectVersion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobjectversion-method)
         """
 
@@ -2750,16 +2728,16 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        ObjectOwnership: ObjectOwnershipType = ...
-    ) -> _Bucket:
+        ObjectOwnership: ObjectOwnershipType = ...,
+    ) -> "_Bucket":
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcecreate_bucket-method)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/service_resource.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/service_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -168,14 +168,15 @@
     "ServiceResourceBucketsCollection",
     "BucketMultipartUploadsCollection",
     "BucketObjectVersionsCollection",
     "BucketObjectsCollection",
     "MultipartUploadPartsCollection",
 )
 
+
 class ServiceResourceBucketsCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.buckets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#serviceresourcebucketscollection)
     """
 
     def all(self) -> "ServiceResourceBucketsCollection":
@@ -230,14 +231,15 @@
         """
         A generator which yields Buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.buckets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#serviceresourcebucketscollection)
         """
 
+
 class BucketMultipartUploadsCollection(AIOResourceCollection):
     def all(self) -> "BucketMultipartUploadsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -246,15 +248,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
     ) -> "BucketMultipartUploadsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "BucketMultipartUploadsCollection":
         """
@@ -277,14 +279,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUpload"]:
         """
         A generator which yields MultipartUploads.
         """
 
+
 class BucketObjectVersionsCollection(AIOResourceCollection):
     def all(self) -> "BucketObjectVersionsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -294,28 +297,28 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> "BucketObjectVersionsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectVersionsCollection":
         """
@@ -338,14 +341,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["ObjectVersion"]:
         """
         A generator which yields ObjectVersions.
         """
 
+
 class BucketObjectsCollection(AIOResourceCollection):
     def all(self) -> "BucketObjectsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -354,28 +358,28 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
     ) -> "BucketObjectsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> List[DeleteObjectsOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectsCollection":
         """
@@ -398,14 +402,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["ObjectSummary"]:
         """
         A generator which yields ObjectSummarys.
         """
 
+
 class MultipartUploadPartsCollection(AIOResourceCollection):
     def all(self) -> "MultipartUploadPartsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -413,15 +418,15 @@
         *,
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
+        SSECustomerKeyMD5: str = ...,
     ) -> "MultipartUploadPartsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     def limit(self, count: int) -> "MultipartUploadPartsCollection":
         """
@@ -444,23 +449,25 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUploadPart"]:
         """
         A generator which yields MultipartUploadParts.
         """
 
+
 class BucketAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketacl)
     """
 
     owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketaclbucket-method)
@@ -491,15 +498,15 @@
         AccessControlPolicy: AccessControlPolicyTypeDef = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketaclput-method)
         """
@@ -510,24 +517,27 @@
         BucketAcl
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketaclreload-method)
         """
 
+
 _BucketAcl = BucketAcl
 
+
 class BucketCors(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcors)
     """
 
     cors_rules: Awaitable[List[CORSRuleBucketCorsTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsbucket-method)
@@ -560,15 +570,15 @@
         """
 
     async def put(
         self,
         *,
         CORSConfiguration: CORSConfigurationBucketCorsTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsput-method)
         """
@@ -579,24 +589,27 @@
         BucketCors
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsreload-method)
         """
 
+
 _BucketCors = BucketCors
 
+
 class BucketLifecycle(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycle)
     """
 
     rules: Awaitable[List[RuleBucketLifecycleTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecyclebucket-method)
@@ -629,15 +642,15 @@
         """
 
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: LifecycleConfigurationBucketLifecycleTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleput-method)
         """
@@ -648,24 +661,27 @@
         BucketLifecycle
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecyclereload-method)
         """
 
+
 _BucketLifecycle = BucketLifecycle
 
+
 class BucketLifecycleConfiguration(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
     rules: Awaitable[List[LifecycleRuleBucketLifecycleConfigurationTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationbucket-method)
@@ -698,15 +714,15 @@
         """
 
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         LifecycleConfiguration: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationput-method)
         """
@@ -717,24 +733,27 @@
         attributes of the BucketLifecycleConfiguration
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationreload-method)
         """
 
+
 _BucketLifecycleConfiguration = BucketLifecycleConfiguration
 
+
 class BucketLogging(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLogging)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlogging)
     """
 
     logging_enabled: Awaitable[LoggingEnabledResponseTypeDef]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingbucket-method)
@@ -759,15 +778,15 @@
         """
 
     async def put(
         self,
         *,
         BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingput-method)
         """
@@ -778,29 +797,32 @@
         BucketLogging
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingreload-method)
         """
 
+
 _BucketLogging = BucketLogging
 
+
 class BucketNotification(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotification)
     """
 
     topic_configurations: Awaitable[List[TopicConfigurationBucketNotificationTypeDef]]
     queue_configurations: Awaitable[List[QueueConfigurationBucketNotificationTypeDef]]
     lambda_function_configurations: Awaitable[
         List[LambdaFunctionConfigurationBucketNotificationTypeDef]
     ]
     event_bridge_configuration: Awaitable[Dict[str, Any]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationbucket-method)
@@ -825,15 +847,15 @@
         """
 
     async def put(
         self,
         *,
         NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,
         ExpectedBucketOwner: str = ...,
-        SkipDestinationValidation: bool = ...
+        SkipDestinationValidation: bool = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationput-method)
         """
@@ -844,24 +866,27 @@
         attributes of the BucketNotification
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationreload-method)
         """
 
+
 _BucketNotification = BucketNotification
 
+
 class BucketPolicy(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketPolicy)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicy)
     """
 
     policy: Awaitable[str]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketPolicy.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicybucket-method)
@@ -895,15 +920,15 @@
 
     async def put(
         self,
         *,
         Policy: str,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ConfirmRemoveSelfBucketAccess: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         Applies an Amazon S3 bucket policy to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketPolicy.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicyput-method)
         """
@@ -914,24 +939,27 @@
         BucketPolicy
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketPolicy.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicyreload-method)
         """
 
+
 _BucketPolicy = BucketPolicy
 
+
 class BucketRequestPayment(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketRequestPayment)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpayment)
     """
 
     payer: Awaitable[PayerType]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketRequestPayment.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpaymentbucket-method)
@@ -956,15 +984,15 @@
         """
 
     async def put(
         self,
         *,
         RequestPaymentConfiguration: RequestPaymentConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketRequestPayment.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpaymentput-method)
         """
@@ -975,24 +1003,27 @@
         of the BucketRequestPayment
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketRequestPayment.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpaymentreload-method)
         """
 
+
 _BucketRequestPayment = BucketRequestPayment
 
+
 class BucketTagging(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketTagging)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettagging)
     """
 
     tag_set: Awaitable[List[TagTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettaggingbucket-method)
@@ -1025,15 +1056,15 @@
         """
 
     async def put(
         self,
         *,
         Tagging: TaggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettaggingput-method)
         """
@@ -1044,40 +1075,43 @@
         BucketTagging
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettaggingreload-method)
         """
 
+
 _BucketTagging = BucketTagging
 
+
 class BucketVersioning(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketVersioning)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioning)
     """
 
     status: Awaitable[BucketVersioningStatusType]
     mfa_delete: Awaitable[MFADeleteStatusType]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningbucket-method)
         """
 
     async def enable(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.enable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningenable-method)
         """
@@ -1102,15 +1136,15 @@
 
     async def put(
         self,
         *,
         VersioningConfiguration: VersioningConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningput-method)
         """
@@ -1126,36 +1160,39 @@
         """
 
     async def suspend(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         MFA: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketVersioning.suspend)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioningsuspend-method)
         """
 
+
 _BucketVersioning = BucketVersioning
 
+
 class BucketWebsite(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketWebsite)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsite)
     """
 
     redirect_all_requests_to: Awaitable[RedirectAllRequestsToResponseTypeDef]
     index_document: Awaitable[IndexDocumentResponseTypeDef]
     error_document: Awaitable[ErrorDocumentResponseTypeDef]
     routing_rules: Awaitable[List[RoutingRuleTypeDef]]
     bucket_name: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsitebucket-method)
@@ -1188,15 +1225,15 @@
         """
 
     async def put(
         self,
         *,
         WebsiteConfiguration: WebsiteConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsiteput-method)
         """
@@ -1207,16 +1244,18 @@
         BucketWebsite
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsitereload-method)
         """
 
+
 _BucketWebsite = BucketWebsite
 
+
 class MultipartUploadPart(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUploadPart)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpart)
     """
 
     last_modified: Awaitable[datetime]
@@ -1226,14 +1265,15 @@
     checksum_crc32_c: Awaitable[str]
     checksum_sha1: Awaitable[str]
     checksum_sha256: Awaitable[str]
     bucket_name: str
     object_key: str
     multipart_upload_id: str
     part_number: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def MultipartUpload(self) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpartmultipartupload-method)
@@ -1252,15 +1292,15 @@
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> UploadPartCopyOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.copy_from)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpartcopy_from-method)
         """
@@ -1284,36 +1324,39 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> UploadPartOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpartupload-method)
         """
 
+
 _MultipartUploadPart = MultipartUploadPart
 
+
 class ObjectAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectacl)
     """
 
     owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     request_charged: Awaitable[Literal["requester"]]
     bucket_name: str
     object_key: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectaclobject-method)
@@ -1346,15 +1389,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectAclOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectaclput-method)
         """
@@ -1365,16 +1408,18 @@
         ObjectAcl
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectaclreload-method)
         """
 
+
 _ObjectAcl = ObjectAcl
 
+
 class ObjectVersion(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectVersion)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversion)
     """
 
     e_tag: Awaitable[str]
@@ -1386,14 +1431,15 @@
     is_latest: Awaitable[bool]
     last_modified: Awaitable[datetime]
     owner: Awaitable[OwnerResponseTypeDef]
     restore_status: Awaitable[RestoreStatusResponseTypeDef]
     bucket_name: str
     object_key: str
     id: str
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversionobject-method)
@@ -1401,15 +1447,15 @@
 
     async def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversiondelete-method)
         """
@@ -1430,15 +1476,15 @@
         ResponseExpires: TimestampTypeDef = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.get)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversionget-method)
         """
@@ -1461,27 +1507,29 @@
         Range: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> HeadObjectOutputTypeDef:
         """
         The `HEAD` operation retrieves metadata from an object without returning the
         object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.head)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversionhead-method)
         """
 
+
 _ObjectVersion = ObjectVersion
 
+
 class MultipartUpload(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUpload)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartupload)
     """
 
     upload_id: Awaitable[str]
@@ -1491,24 +1539,25 @@
     owner: Awaitable[OwnerTypeDef]
     initiator: Awaitable[InitiatorResponseTypeDef]
     checksum_algorithm: Awaitable[ChecksumAlgorithmType]
     bucket_name: str
     object_key: str
     id: str
     parts: MultipartUploadPartsCollection
+    meta: Awaitable["S3ResourceMeta"]
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadobject-method)
         """
 
-    async def Part(self, part_number: str) -> _MultipartUploadPart:
+    async def Part(self, part_number: str) -> "_MultipartUploadPart":
         """
         Creates a MultipartUploadPart resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadpart-method)
         """
 
@@ -1530,16 +1579,16 @@
         ChecksumCRC32C: str = ...,
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
-        SSECustomerKeyMD5: str = ...
-    ) -> _Object:
+        SSECustomerKeyMD5: str = ...,
+    ) -> "_Object":
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.complete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadcomplete-method)
         """
 
@@ -1547,16 +1596,18 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartuploadget_available_subresources-method)
         """
 
+
 _MultipartUpload = MultipartUpload
 
+
 class Object(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Object)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#object)
     """
 
     delete_marker: Awaitable[bool]
@@ -1591,16 +1642,17 @@
     replication_status: Awaitable[ReplicationStatusType]
     parts_count: Awaitable[int]
     object_lock_mode: Awaitable[ObjectLockModeType]
     object_lock_retain_until_date: Awaitable[datetime]
     object_lock_legal_hold_status: Awaitable[ObjectLockLegalHoldStatusType]
     bucket_name: str
     key: str
+    meta: Awaitable["S3ResourceMeta"]
 
-    async def Acl(self) -> _ObjectAcl:
+    async def Acl(self) -> "_ObjectAcl":
         """
         Creates a ObjectAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.Acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectacl-method)
         """
 
@@ -1608,23 +1660,23 @@
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectbucket-method)
         """
 
-    async def MultipartUpload(self, id: str) -> _MultipartUpload:
+    async def MultipartUpload(self, id: str) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectmultipartupload-method)
         """
 
-    async def Version(self, id: str) -> _ObjectVersion:
+    async def Version(self, id: str) -> "_ObjectVersion":
         """
         Creates a ObjectVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.Version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectversion-method)
         """
 
@@ -1680,15 +1732,15 @@
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.copy_from)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectcopy_from-method)
         """
@@ -1696,15 +1748,15 @@
     async def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectdelete-method)
         """
@@ -1754,15 +1806,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.get)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectget-method)
         """
@@ -1801,16 +1853,16 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> _MultipartUpload:
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
+    ) -> "_MultipartUpload":
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectinitiate_multipart_upload-method)
         """
 
@@ -1856,15 +1908,15 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectput-method)
         """
@@ -1881,15 +1933,15 @@
     async def restore_object(
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> RestoreObjectOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.restore_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectrestore_object-method)
         """
@@ -1934,16 +1986,18 @@
         """
         Waits until this Object is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.wait_until_not_exists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectwait_until_not_exists-method)
         """
 
+
 _Object = Object
 
+
 class ObjectSummary(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectSummary)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummary)
     """
 
     last_modified: Awaitable[datetime]
@@ -1951,16 +2005,17 @@
     checksum_algorithm: Awaitable[List[ChecksumAlgorithmType]]
     size: Awaitable[int]
     storage_class: Awaitable[ObjectStorageClassType]
     owner: Awaitable[OwnerTypeDef]
     restore_status: Awaitable[RestoreStatusTypeDef]
     bucket_name: str
     key: str
+    meta: Awaitable["S3ResourceMeta"]
 
-    async def Acl(self) -> _ObjectAcl:
+    async def Acl(self) -> "_ObjectAcl":
         """
         Creates a ObjectAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryacl-method)
         """
 
@@ -1968,31 +2023,31 @@
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarybucket-method)
         """
 
-    async def MultipartUpload(self, id: str) -> _MultipartUpload:
+    async def MultipartUpload(self, id: str) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarymultipartupload-method)
         """
 
-    async def Object(self) -> _Object:
+    async def Object(self) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryobject-method)
         """
 
-    async def Version(self, id: str) -> _ObjectVersion:
+    async def Version(self, id: str) -> "_ObjectVersion":
         """
         Creates a ObjectVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.Version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryversion-method)
         """
 
@@ -2033,15 +2088,15 @@
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ExpectedSourceBucketOwner: str = ...
+        ExpectedSourceBucketOwner: str = ...,
     ) -> CopyObjectOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.copy_from)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarycopy_from-method)
         """
@@ -2049,15 +2104,15 @@
     async def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> DeleteObjectOutputTypeDef:
         """
         Removes an object from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarydelete-method)
         """
@@ -2079,15 +2134,15 @@
         VersionId: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumMode: Literal["ENABLED"] = ...
+        ChecksumMode: Literal["ENABLED"] = ...,
     ) -> GetObjectOutputTypeDef:
         """
         Retrieves an object from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.get)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryget-method)
         """
@@ -2126,16 +2181,16 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> _MultipartUpload:
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
+    ) -> "_MultipartUpload":
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryinitiate_multipart_upload-method)
         """
 
@@ -2181,15 +2236,15 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryput-method)
         """
@@ -2197,15 +2252,15 @@
     async def restore_object(
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
     ) -> RestoreObjectOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.restore_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummaryrestore_object-method)
         """
@@ -2222,117 +2277,120 @@
         """
         Waits until this ObjectSummary is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.wait_until_not_exists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectsummarywait_until_not_exists-method)
         """
 
+
 _ObjectSummary = ObjectSummary
 
+
 class Bucket(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Bucket)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucket)
     """
 
     creation_date: Awaitable[datetime]
     name: str
     multipart_uploads: BucketMultipartUploadsCollection
     object_versions: BucketObjectVersionsCollection
     objects: BucketObjectsCollection
+    meta: Awaitable["S3ResourceMeta"]
 
-    async def Acl(self) -> _BucketAcl:
+    async def Acl(self) -> "_BucketAcl":
         """
         Creates a BucketAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketacl-method)
         """
 
-    async def Cors(self) -> _BucketCors:
+    async def Cors(self) -> "_BucketCors":
         """
         Creates a BucketCors resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Cors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcors-method)
         """
 
-    async def Lifecycle(self) -> _BucketLifecycle:
+    async def Lifecycle(self) -> "_BucketLifecycle":
         """
         Creates a BucketLifecycle resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Lifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycle-method)
         """
 
-    async def LifecycleConfiguration(self) -> _BucketLifecycleConfiguration:
+    async def LifecycleConfiguration(self) -> "_BucketLifecycleConfiguration":
         """
         Creates a BucketLifecycleConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.LifecycleConfiguration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfiguration-method)
         """
 
-    async def Logging(self) -> _BucketLogging:
+    async def Logging(self) -> "_BucketLogging":
         """
         Creates a BucketLogging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlogging-method)
         """
 
-    async def Notification(self) -> _BucketNotification:
+    async def Notification(self) -> "_BucketNotification":
         """
         Creates a BucketNotification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotification-method)
         """
 
-    async def Object(self, key: str) -> _Object:
+    async def Object(self, key: str) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketobject-method)
         """
 
-    async def Policy(self) -> _BucketPolicy:
+    async def Policy(self) -> "_BucketPolicy":
         """
         Creates a BucketPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketpolicy-method)
         """
 
-    async def RequestPayment(self) -> _BucketRequestPayment:
+    async def RequestPayment(self) -> "_BucketRequestPayment":
         """
         Creates a BucketRequestPayment resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.RequestPayment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketrequestpayment-method)
         """
 
-    async def Tagging(self) -> _BucketTagging:
+    async def Tagging(self) -> "_BucketTagging":
         """
         Creates a BucketTagging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#buckettagging-method)
         """
 
-    async def Versioning(self) -> _BucketVersioning:
+    async def Versioning(self) -> "_BucketVersioning":
         """
         Creates a BucketVersioning resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketversioning-method)
         """
 
-    async def Website(self) -> _BucketWebsite:
+    async def Website(self) -> "_BucketWebsite":
         """
         Creates a BucketWebsite resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.Website)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwebsite-method)
         """
 
@@ -2359,15 +2417,15 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        ObjectOwnership: ObjectOwnershipType = ...
+        ObjectOwnership: ObjectOwnershipType = ...,
     ) -> CreateBucketOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.create)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcreate-method)
         """
@@ -2384,15 +2442,15 @@
         self,
         *,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
-        ChecksumAlgorithm: ChecksumAlgorithmType = ...
+        ChecksumAlgorithm: ChecksumAlgorithmType = ...,
     ) -> DeleteObjectsOutputTypeDef:
         """
         This operation enables you to delete multiple objects from a bucket using a
         single HTTP
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.delete_objects)
@@ -2479,16 +2537,16 @@
         SSEKMSEncryptionContext: str = ...,
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: TimestampTypeDef = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
-        ExpectedBucketOwner: str = ...
-    ) -> _Object:
+        ExpectedBucketOwner: str = ...,
+    ) -> "_Object":
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketput_object-method)
         """
 
@@ -2534,167 +2592,174 @@
         """
         Waits until this Bucket is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.wait_until_not_exists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketwait_until_not_exists-method)
         """
 
+
 _Bucket = Bucket
 
+
 class S3ResourceMeta(ResourceMeta):
     client: S3Client
 
+
 class S3ServiceResource(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/)
     """
 
     meta: "S3ResourceMeta"
     buckets: ServiceResourceBucketsCollection
 
-    async def Bucket(self, name: str) -> _Bucket:
+    async def Bucket(self, name: str) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucket-method)
         """
 
-    async def BucketAcl(self, bucket_name: str) -> _BucketAcl:
+    async def BucketAcl(self, bucket_name: str) -> "_BucketAcl":
         """
         Creates a BucketAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketacl-method)
         """
 
-    async def BucketCors(self, bucket_name: str) -> _BucketCors:
+    async def BucketCors(self, bucket_name: str) -> "_BucketCors":
         """
         Creates a BucketCors resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketcors-method)
         """
 
-    async def BucketLifecycle(self, bucket_name: str) -> _BucketLifecycle:
+    async def BucketLifecycle(self, bucket_name: str) -> "_BucketLifecycle":
         """
         Creates a BucketLifecycle resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketlifecycle-method)
         """
 
-    async def BucketLifecycleConfiguration(self, bucket_name: str) -> _BucketLifecycleConfiguration:
+    async def BucketLifecycleConfiguration(
+        self, bucket_name: str
+    ) -> "_BucketLifecycleConfiguration":
         """
         Creates a BucketLifecycleConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketlifecycleconfiguration-method)
         """
 
-    async def BucketLogging(self, bucket_name: str) -> _BucketLogging:
+    async def BucketLogging(self, bucket_name: str) -> "_BucketLogging":
         """
         Creates a BucketLogging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLogging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketlogging-method)
         """
 
-    async def BucketNotification(self, bucket_name: str) -> _BucketNotification:
+    async def BucketNotification(self, bucket_name: str) -> "_BucketNotification":
         """
         Creates a BucketNotification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketnotification-method)
         """
 
-    async def BucketPolicy(self, bucket_name: str) -> _BucketPolicy:
+    async def BucketPolicy(self, bucket_name: str) -> "_BucketPolicy":
         """
         Creates a BucketPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketPolicy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketpolicy-method)
         """
 
-    async def BucketRequestPayment(self, bucket_name: str) -> _BucketRequestPayment:
+    async def BucketRequestPayment(self, bucket_name: str) -> "_BucketRequestPayment":
         """
         Creates a BucketRequestPayment resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketRequestPayment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketrequestpayment-method)
         """
 
-    async def BucketTagging(self, bucket_name: str) -> _BucketTagging:
+    async def BucketTagging(self, bucket_name: str) -> "_BucketTagging":
         """
         Creates a BucketTagging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketTagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebuckettagging-method)
         """
 
-    async def BucketVersioning(self, bucket_name: str) -> _BucketVersioning:
+    async def BucketVersioning(self, bucket_name: str) -> "_BucketVersioning":
         """
         Creates a BucketVersioning resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketVersioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketversioning-method)
         """
 
-    async def BucketWebsite(self, bucket_name: str) -> _BucketWebsite:
+    async def BucketWebsite(self, bucket_name: str) -> "_BucketWebsite":
         """
         Creates a BucketWebsite resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketWebsite)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcebucketwebsite-method)
         """
 
-    async def MultipartUpload(self, bucket_name: str, object_key: str, id: str) -> _MultipartUpload:
+    async def MultipartUpload(
+        self, bucket_name: str, object_key: str, id: str
+    ) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcemultipartupload-method)
         """
 
     async def MultipartUploadPart(
         self, bucket_name: str, object_key: str, multipart_upload_id: str, part_number: str
-    ) -> _MultipartUploadPart:
+    ) -> "_MultipartUploadPart":
         """
         Creates a MultipartUploadPart resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.MultipartUploadPart)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcemultipartuploadpart-method)
         """
 
-    async def Object(self, bucket_name: str, key: str) -> _Object:
+    async def Object(self, bucket_name: str, key: str) -> "_Object":
         """
         Creates a Object resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.Object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobject-method)
         """
 
-    async def ObjectAcl(self, bucket_name: str, object_key: str) -> _ObjectAcl:
+    async def ObjectAcl(self, bucket_name: str, object_key: str) -> "_ObjectAcl":
         """
         Creates a ObjectAcl resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobjectacl-method)
         """
 
-    async def ObjectSummary(self, bucket_name: str, key: str) -> _ObjectSummary:
+    async def ObjectSummary(self, bucket_name: str, key: str) -> "_ObjectSummary":
         """
         Creates a ObjectSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectSummary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobjectsummary-method)
         """
 
-    async def ObjectVersion(self, bucket_name: str, object_key: str, id: str) -> _ObjectVersion:
+    async def ObjectVersion(self, bucket_name: str, object_key: str, id: str) -> "_ObjectVersion":
         """
         Creates a ObjectVersion resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectVersion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourceobjectversion-method)
         """
 
@@ -2706,16 +2771,16 @@
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
-        ObjectOwnership: ObjectOwnershipType = ...
-    ) -> _Bucket:
+        ObjectOwnership: ObjectOwnershipType = ...,
+    ) -> "_Bucket":
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#s3serviceresourcecreate_bucket-method)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/type_defs.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 else:
     from typing_extensions import TypedDict
 try:
     from boto3.s3.transfer import TransferConfig
 except ImportError:
     from builtins import object as TransferConfig
 
-
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
     "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "AccessControlTranslationTypeDef",
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/type_defs.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/waiter.py` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/waiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from .type_defs import TimestampTypeDef, WaiterConfigTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BucketExistsWaiter",
     "BucketNotExistsWaiter",
     "ObjectExistsWaiter",
     "ObjectNotExistsWaiter",
 )
 
@@ -54,15 +53,15 @@
     """
 
     async def wait(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.BucketExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#bucketexistswaiter)
         """
 
 
@@ -73,15 +72,15 @@
     """
 
     async def wait(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.BucketNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#bucketnotexistswaiter)
         """
 
 
@@ -105,15 +104,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.ObjectExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#objectexistswaiter)
         """
 
 
@@ -137,13 +136,13 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.ObjectNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#objectnotexistswaiter)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3/waiter.pyi` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3/waiter.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
 
     async def wait(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.BucketExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#bucketexistswaiter)
         """
 
 class BucketNotExistsWaiter(AIOWaiter):
@@ -70,15 +70,15 @@
     """
 
     async def wait(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.BucketNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#bucketnotexistswaiter)
         """
 
 class ObjectExistsWaiter(AIOWaiter):
@@ -101,15 +101,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.ObjectExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#objectexistswaiter)
         """
 
 class ObjectNotExistsWaiter(AIOWaiter):
@@ -132,13 +132,13 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Waiter.ObjectNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/waiters/#objectnotexistswaiter)
         """
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/PKG-INFO` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.S3 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.S3 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/
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
 
 <a id="types-aiobotocore-s3"></a>
 
 # types-aiobotocore-s3
 
 [![PyPI - types-aiobotocore-s3](https://img.shields.io/pypi/v/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3)](https://pepy.tech/project/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
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
 [types-aiobotocore-s3 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-s3-2.9.0/types_aiobotocore_s3.egg-info/SOURCES.txt` & `types-aiobotocore-s3-2.9.1/types_aiobotocore_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

