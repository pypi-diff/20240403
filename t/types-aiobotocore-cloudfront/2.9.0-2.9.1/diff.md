# Comparing `tmp/types-aiobotocore-cloudfront-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudfront-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudfront-2.9.0.tar", last modified: Wed Dec 13 19:58:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudfront-2.9.1.tar", last modified: Thu Jan 18 01:20:16 2024, max compression
```

## Comparing `types-aiobotocore-cloudfront-2.9.0.tar` & `types-aiobotocore-cloudfront-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.601972 types-aiobotocore-cloudfront-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15016 2023-12-13 19:58:49.601972 types-aiobotocore-cloudfront-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:49.601972 types-aiobotocore-cloudfront-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:42:24.000000 types-aiobotocore-cloudfront-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.601972 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86877 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    86873 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   105130 2023-12-13 19:42:29.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   105129 2023-12-13 19:42:27.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:25.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-13 19:42:26.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:49.601972 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15016 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:49.000000 types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.349461 types-aiobotocore-cloudfront-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-01-18 01:20:16.349461 types-aiobotocore-cloudfront-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:16.349461 types-aiobotocore-cloudfront-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.345461 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86889 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   105129 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105129 2024-01-18 01:04:25.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:22.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-01-18 01:04:23.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:16.349461 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-01-18 01:20:16.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-18 01:20:16.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:16.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:16.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:16.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:16.000000 types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/LICENSE` & `types-aiobotocore-cloudfront-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudfront-2.9.0/PKG-INFO` & `types-aiobotocore-cloudfront-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudFront 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudFront 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
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
 
 <a id="types-aiobotocore-cloudfront"></a>
 
 # types-aiobotocore-cloudfront
 
 [![PyPI - types-aiobotocore-cloudfront](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [types-aiobotocore-cloudfront docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/README.md` & `types-aiobotocore-cloudfront-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [types-aiobotocore-cloudfront docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/setup.py` & `types-aiobotocore-cloudfront-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudfront",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudFront 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudFront 2.9.1 service generated with"
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
     keywords="aiobotocore cloudfront type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudfront": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/__init__.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     DistributionDeployedWaiter,
     InvalidationCompletedWaiter,
     StreamingDistributionDeployedWaiter,
 )
 
 Client = CloudFrontClient
 
-
 __all__ = (
     "Client",
     "CloudFrontClient",
     "DistributionDeployedWaiter",
     "InvalidationCompletedWaiter",
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/__init__.pyi` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/__main__.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFront 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudFront 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/client.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudFrontClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -375,15 +374,15 @@
     async def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
         IfMatch: str = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
@@ -548,15 +547,15 @@
 
     async def create_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef],
         Fields: Sequence[str],
         Name: str,
-        SamplingRate: int
+        SamplingRate: int,
     ) -> CreateRealtimeLogConfigResultTypeDef:
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_realtime_log_config)
         """
@@ -1141,15 +1140,15 @@
 
     async def list_distributions_by_realtime_log_config(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         RealtimeLogConfigName: str = ...,
-        RealtimeLogConfigArn: str = ...
+        RealtimeLogConfigArn: str = ...,
     ) -> ListDistributionsByRealtimeLogConfigResultTypeDef:
         """
         Gets a list of distributions that have a cache behavior that's associated with
         the specified real-time log
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)
@@ -1362,29 +1361,29 @@
         """
 
     async def update_cloud_front_origin_access_identity(
         self,
         *,
         CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Update an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     async def update_continuous_deployment_policy(
         self,
         *,
         ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_continuous_deployment_policy)
         """
@@ -1411,44 +1410,44 @@
         """
 
     async def update_field_level_encryption_config(
         self,
         *,
         FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_config)
         """
 
     async def update_field_level_encryption_profile(
         self,
         *,
         FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_profile)
         """
 
     async def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: BlobTypeDef
+        FunctionCode: BlobTypeDef,
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_function)
         """
@@ -1474,29 +1473,29 @@
         """
 
     async def update_origin_access_control(
         self,
         *,
         OriginAccessControlConfig: OriginAccessControlConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginAccessControlResultTypeDef:
         """
         Updates a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_access_control)
         """
 
     async def update_origin_request_policy(
         self,
         *,
         OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_request_policy)
         """
@@ -1514,43 +1513,43 @@
     async def update_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef] = ...,
         Fields: Sequence[str] = ...,
         Name: str = ...,
         ARN: str = ...,
-        SamplingRate: int = ...
+        SamplingRate: int = ...,
     ) -> UpdateRealtimeLogConfigResultTypeDef:
         """
         Updates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_realtime_log_config)
         """
 
     async def update_response_headers_policy(
         self,
         *,
         ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_response_headers_policy)
         """
 
     async def update_streaming_distribution(
         self,
         *,
         StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_streaming_distribution)
         """
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/client.pyi` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     async def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
         IfMatch: str = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
@@ -544,15 +544,15 @@
 
     async def create_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef],
         Fields: Sequence[str],
         Name: str,
-        SamplingRate: int
+        SamplingRate: int,
     ) -> CreateRealtimeLogConfigResultTypeDef:
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_realtime_log_config)
         """
@@ -1137,15 +1137,15 @@
 
     async def list_distributions_by_realtime_log_config(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         RealtimeLogConfigName: str = ...,
-        RealtimeLogConfigArn: str = ...
+        RealtimeLogConfigArn: str = ...,
     ) -> ListDistributionsByRealtimeLogConfigResultTypeDef:
         """
         Gets a list of distributions that have a cache behavior that's associated with
         the specified real-time log
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)
@@ -1358,29 +1358,29 @@
         """
 
     async def update_cloud_front_origin_access_identity(
         self,
         *,
         CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Update an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     async def update_continuous_deployment_policy(
         self,
         *,
         ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_continuous_deployment_policy)
         """
@@ -1407,44 +1407,44 @@
         """
 
     async def update_field_level_encryption_config(
         self,
         *,
         FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_config)
         """
 
     async def update_field_level_encryption_profile(
         self,
         *,
         FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_profile)
         """
 
     async def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: BlobTypeDef
+        FunctionCode: BlobTypeDef,
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_function)
         """
@@ -1470,29 +1470,29 @@
         """
 
     async def update_origin_access_control(
         self,
         *,
         OriginAccessControlConfig: OriginAccessControlConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginAccessControlResultTypeDef:
         """
         Updates a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_access_control)
         """
 
     async def update_origin_request_policy(
         self,
         *,
         OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_request_policy)
         """
@@ -1510,43 +1510,43 @@
     async def update_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef] = ...,
         Fields: Sequence[str] = ...,
         Name: str = ...,
         ARN: str = ...,
-        SamplingRate: int = ...
+        SamplingRate: int = ...,
     ) -> UpdateRealtimeLogConfigResultTypeDef:
         """
         Updates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_realtime_log_config)
         """
 
     async def update_response_headers_policy(
         self,
         *,
         ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_response_headers_policy)
         """
 
     async def update_streaming_distribution(
         self,
         *,
         StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_streaming_distribution)
         """
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/literals.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/literals.py`

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
     "CachePolicyCookieBehaviorType",
     "CachePolicyHeaderBehaviorType",
     "CachePolicyQueryStringBehaviorType",
     "CachePolicyTypeType",
     "CertificateSourceType",
     "ContinuousDeploymentPolicyTypeType",
@@ -66,15 +65,14 @@
     "CloudFrontServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
-
 CachePolicyCookieBehaviorType = Literal["all", "allExcept", "none", "whitelist"]
 CachePolicyHeaderBehaviorType = Literal["none", "whitelist"]
 CachePolicyQueryStringBehaviorType = Literal["all", "allExcept", "none", "whitelist"]
 CachePolicyTypeType = Literal["custom", "managed"]
 CertificateSourceType = Literal["acm", "cloudfront", "iam"]
 ContinuousDeploymentPolicyTypeType = Literal["SingleHeader", "SingleWeight"]
 DistributionDeployedWaiterName = Literal["distribution_deployed"]
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/literals.pyi` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/paginator.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
     "ListInvalidationsPaginator",
     "ListKeyValueStoresPaginator",
     "ListStreamingDistributionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/paginator.pyi` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/type_defs.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasICPRecordalTypeDef",
     "AliasesTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
     "BlobTypeDef",
     "TrustedKeyGroupsTypeDef",
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/type_defs.pyi` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/waiter.py` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront/waiter.pyi` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/PKG-INFO` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudFront 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudFront 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
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
 
 <a id="types-aiobotocore-cloudfront"></a>
 
 # types-aiobotocore-cloudfront
 
 [![PyPI - types-aiobotocore-cloudfront](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [types-aiobotocore-cloudfront docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudfront-2.9.0/types_aiobotocore_cloudfront.egg-info/SOURCES.txt` & `types-aiobotocore-cloudfront-2.9.1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

