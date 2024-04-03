# Comparing `tmp/types-aiobotocore-cloudfront-keyvaluestore-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudfront-keyvaluestore-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudfront-keyvaluestore-2.9.0.tar", last modified: Wed Dec 13 19:58:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudfront-keyvaluestore-2.9.1.tar", last modified: Thu Jan 18 01:20:16 2024, max compression
```

## Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0.tar` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.233975 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2023-12-13 19:58:49.233975 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12304 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:49.233975 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.233975 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.233975 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.013463 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-01-18 01:20:16.013463 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12304 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:16.013463 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.013463 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-01-18 01:04:26.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-01-18 01:04:26.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-18 01:04:26.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-18 01:04:26.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.013463 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-01-18 01:20:15.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-18 01:20:15.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:15.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:15.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:15.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-18 01:20:15.000000 types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/LICENSE` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/PKG-INFO` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront-keyvaluestore
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/
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
 
 <a id="types-aiobotocore-cloudfront-keyvaluestore"></a>
 
 # types-aiobotocore-cloudfront-keyvaluestore
 
 [![PyPI - types-aiobotocore-cloudfront-keyvaluestore](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront-keyvaluestore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront-keyvaluestore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront-keyvaluestore)](https://pepy.tech/project/types-aiobotocore-cloudfront-keyvaluestore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFrontKeyValueStore 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore)
+[aiobotocore.CloudFrontKeyValueStore 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore)
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
 [types-aiobotocore-cloudfront-keyvaluestore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/README.md` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront-keyvaluestore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront-keyvaluestore)](https://pepy.tech/project/types-aiobotocore-cloudfront-keyvaluestore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFrontKeyValueStore 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore)
+[aiobotocore.CloudFrontKeyValueStore 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore)
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
 [types-aiobotocore-cloudfront-keyvaluestore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/setup.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudfront-keyvaluestore",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudfront_keyvaluestore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.1 service generated with"
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
         "aiobotocore cloudfront-keyvaluestore type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudfront_keyvaluestore": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/__init__.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import CloudFrontKeyValueStoreClient
 from .paginator import ListKeysPaginator
 
 Client = CloudFrontKeyValueStoreClient
 
-
 __all__ = ("Client", "CloudFrontKeyValueStoreClient", "ListKeysPaginator")
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/__init__.pyi` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/__main__.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore\nOther"
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

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/client.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudFrontKeyValueStoreClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -155,15 +154,15 @@
 
     async def update_keys(
         self,
         *,
         KvsARN: str,
         IfMatch: str,
         Puts: Sequence[PutKeyRequestListItemTypeDef] = ...,
-        Deletes: Sequence[DeleteKeyRequestListItemTypeDef] = ...
+        Deletes: Sequence[DeleteKeyRequestListItemTypeDef] = ...,
     ) -> UpdateKeysResponseTypeDef:
         """
         Puts or Deletes multiple key value pairs in a single, all-or-nothing operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore.Client.update_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/client/#update_keys)
         """
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/client.pyi` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
     async def update_keys(
         self,
         *,
         KvsARN: str,
         IfMatch: str,
         Puts: Sequence[PutKeyRequestListItemTypeDef] = ...,
-        Deletes: Sequence[DeleteKeyRequestListItemTypeDef] = ...
+        Deletes: Sequence[DeleteKeyRequestListItemTypeDef] = ...,
     ) -> UpdateKeysResponseTypeDef:
         """
         Puts or Deletes multiple key value pairs in a single, all-or-nothing operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore.Client.update_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/client/#update_keys)
         """
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/literals.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListKeysPaginatorName",
     "CloudFrontKeyValueStoreServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListKeysPaginatorName = Literal["list_keys"]
 CloudFrontKeyValueStoreServiceName = Literal["cloudfront-keyvaluestore"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/literals.pyi` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/paginator.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListKeysResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListKeysPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/paginator.pyi` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/type_defs.py` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteKeyRequestListItemTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeKeyValueStoreRequestRequestTypeDef",
     "GetKeyRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore/type_defs.pyi` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/PKG-INFO` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront-keyvaluestore
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudFrontKeyValueStore 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/
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
 
 <a id="types-aiobotocore-cloudfront-keyvaluestore"></a>
 
 # types-aiobotocore-cloudfront-keyvaluestore
 
 [![PyPI - types-aiobotocore-cloudfront-keyvaluestore](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront-keyvaluestore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront-keyvaluestore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront-keyvaluestore)](https://pepy.tech/project/types-aiobotocore-cloudfront-keyvaluestore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFrontKeyValueStore 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore)
+[aiobotocore.CloudFrontKeyValueStore 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore)
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
 [types-aiobotocore-cloudfront-keyvaluestore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront_keyvaluestore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudfront-keyvaluestore-2.9.0/types_aiobotocore_cloudfront_keyvaluestore.egg-info/SOURCES.txt` & `types-aiobotocore-cloudfront-keyvaluestore-2.9.1/types_aiobotocore_cloudfront_keyvaluestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

