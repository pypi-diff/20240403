# Comparing `tmp/types-aiobotocore-marketplacecommerceanalytics-2.9.0.tar.gz` & `tmp/types-aiobotocore-marketplacecommerceanalytics-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplacecommerceanalytics-2.9.0.tar", last modified: Wed Dec 13 19:59:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplacecommerceanalytics-2.9.1.tar", last modified: Thu Jan 18 01:21:13 2024, max compression
```

## Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0.tar` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:51.937474 types-aiobotocore-marketplacecommerceanalytics-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2023-12-13 19:59:51.937474 types-aiobotocore-marketplacecommerceanalytics-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:51.937474 types-aiobotocore-marketplacecommerceanalytics-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-12-13 19:49:46.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:51.937474 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:47.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:51.937474 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2023-12-13 19:59:51.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-13 19:59:51.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:51.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:51.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:51.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-13 19:59:51.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:13.941192 types-aiobotocore-marketplacecommerceanalytics-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-01-18 01:21:13.941192 types-aiobotocore-marketplacecommerceanalytics-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:13.941192 types-aiobotocore-marketplacecommerceanalytics-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-01-18 01:11:31.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:13.937192 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:32.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:13.941192 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-01-18 01:21:13.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-18 01:21:13.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:13.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:13.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:13.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 01:21:13.000000 types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/LICENSE` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/PKG-INFO` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplacecommerceanalytics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/
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
 
 <a id="types-aiobotocore-marketplacecommerceanalytics"></a>
 
 # types-aiobotocore-marketplacecommerceanalytics
 
 [![PyPI - types-aiobotocore-marketplacecommerceanalytics](https://img.shields.io/pypi/v/types-aiobotocore-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplacecommerceanalytics)](https://pepy.tech/project/types-aiobotocore-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCommerceAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[aiobotocore.MarketplaceCommerceAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [types-aiobotocore-marketplacecommerceanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/README.md` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplacecommerceanalytics)](https://pepy.tech/project/types-aiobotocore-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCommerceAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[aiobotocore.MarketplaceCommerceAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [types-aiobotocore-marketplacecommerceanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/setup.py` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplacecommerceanalytics",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_marketplacecommerceanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.1 service generated with"
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
         "aiobotocore marketplacecommerceanalytics type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_marketplacecommerceanalytics": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/__init__.py` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import MarketplaceCommerceAnalyticsClient
 
 Client = MarketplaceCommerceAnalyticsClient
 
-
 __all__ = ("Client", "MarketplaceCommerceAnalyticsClient")
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/__init__.pyi` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/__main__.py` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics\nOther"
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

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/client.py` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         *,
         dataSetType: DataSetTypeType,
         dataSetPublicationDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
-        customerDefinedValues: Mapping[str, str] = ...
+        customerDefinedValues: Mapping[str, str] = ...,
     ) -> GenerateDataSetResultTypeDef:
         """
         Given a data set type and data set publication date, asynchronously publishes
         the requested data set to the specified S3 bucket and notifies the specified
         SNS topic once the data is
         available.
 
@@ -116,15 +116,15 @@
         *,
         dataSetType: SupportDataSetTypeType,
         fromDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
-        customerDefinedValues: Mapping[str, str] = ...
+        customerDefinedValues: Mapping[str, str] = ...,
     ) -> StartSupportDataExportResultTypeDef:
         """
         *This target has been deprecated.* Given a data set type and a from date,
         asynchronously publishes the requested customer support data to the specified
         S3 bucket and notifies the specified SNS topic once the data is
         available.
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/client.pyi` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         *,
         dataSetType: DataSetTypeType,
         dataSetPublicationDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
-        customerDefinedValues: Mapping[str, str] = ...
+        customerDefinedValues: Mapping[str, str] = ...,
     ) -> GenerateDataSetResultTypeDef:
         """
         Given a data set type and data set publication date, asynchronously publishes
         the requested data set to the specified S3 bucket and notifies the specified
         SNS topic once the data is
         available.
 
@@ -113,15 +113,15 @@
         *,
         dataSetType: SupportDataSetTypeType,
         fromDate: TimestampTypeDef,
         roleNameArn: str,
         destinationS3BucketName: str,
         snsTopicArn: str,
         destinationS3Prefix: str = ...,
-        customerDefinedValues: Mapping[str, str] = ...
+        customerDefinedValues: Mapping[str, str] = ...,
     ) -> StartSupportDataExportResultTypeDef:
         """
         *This target has been deprecated.* Given a data set type and a from date,
         asynchronously publishes the requested customer support data to the specified
         S3 bucket and notifies the specified SNS topic once the data is
         available.
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/literals.py` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataSetTypeType",
     "SupportDataSetTypeType",
     "MarketplaceCommerceAnalyticsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DataSetTypeType = Literal[
     "customer_profile_by_geography",
     "customer_profile_by_industry",
     "customer_profile_by_revenue",
     "customer_subscriber_annual_subscriptions",
     "customer_subscriber_hourly_monthly_subscriptions",
     "daily_business_canceled_product_subscribers",
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/literals.pyi` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/type_defs.py` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/type_defs.py`

 * *Files 1% similar despite different names*

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
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "GenerateDataSetRequestRequestTypeDef",
     "StartSupportDataExportRequestRequestTypeDef",
     "GenerateDataSetResultTypeDef",
     "StartSupportDataExportResultTypeDef",
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics/type_defs.pyi` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/PKG-INFO` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplacecommerceanalytics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MarketplaceCommerceAnalytics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/
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
 
 <a id="types-aiobotocore-marketplacecommerceanalytics"></a>
 
 # types-aiobotocore-marketplacecommerceanalytics
 
 [![PyPI - types-aiobotocore-marketplacecommerceanalytics](https://img.shields.io/pypi/v/types-aiobotocore-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplacecommerceanalytics)](https://pepy.tech/project/types-aiobotocore-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCommerceAnalytics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[aiobotocore.MarketplaceCommerceAnalytics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [types-aiobotocore-marketplacecommerceanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplacecommerceanalytics-2.9.0/types_aiobotocore_marketplacecommerceanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-marketplacecommerceanalytics-2.9.1/types_aiobotocore_marketplacecommerceanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

