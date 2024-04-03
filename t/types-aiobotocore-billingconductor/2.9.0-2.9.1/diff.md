# Comparing `tmp/types-aiobotocore-billingconductor-2.9.0.tar.gz` & `tmp/types-aiobotocore-billingconductor-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-billingconductor-2.9.0.tar", last modified: Wed Dec 13 19:58:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-billingconductor-2.9.1.tar", last modified: Thu Jan 18 01:20:10 2024, max compression
```

## Comparing `types-aiobotocore-billingconductor-2.9.0.tar` & `types-aiobotocore-billingconductor-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.206023 types-aiobotocore-billingconductor-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2023-12-13 19:58:43.206023 types-aiobotocore-billingconductor-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13771 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:43.206023 types-aiobotocore-billingconductor-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.206023 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33759 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33755 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10968 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39951 2023-12-13 19:41:47.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39950 2023-12-13 19:41:47.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:46.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.206023 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2023-12-13 19:58:43.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:58:43.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:43.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:43.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:43.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:58:43.000000 types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:10.525488 types-aiobotocore-billingconductor-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-01-18 01:20:10.525488 types-aiobotocore-billingconductor-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:10.525488 types-aiobotocore-billingconductor-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:10.525488 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33777 2024-01-18 01:03:44.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33774 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-01-18 01:03:45.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-01-18 01:03:44.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-01-18 01:03:44.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15030 2024-01-18 01:03:44.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39950 2024-01-18 01:03:45.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39950 2024-01-18 01:03:45.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:43.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:10.525488 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15390 2024-01-18 01:20:10.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:20:10.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:10.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:10.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:10.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:20:10.000000 types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/LICENSE` & `types-aiobotocore-billingconductor-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-billingconductor-2.9.0/PKG-INFO` & `types-aiobotocore-billingconductor-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-billingconductor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BillingConductor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BillingConductor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/
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
 
 <a id="types-aiobotocore-billingconductor"></a>
 
 # types-aiobotocore-billingconductor
 
 [![PyPI - types-aiobotocore-billingconductor](https://img.shields.io/pypi/v/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingConductor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[aiobotocore.BillingConductor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [types-aiobotocore-billingconductor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/README.md` & `types-aiobotocore-billingconductor-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingConductor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[aiobotocore.BillingConductor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [types-aiobotocore-billingconductor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/setup.py` & `types-aiobotocore-billingconductor-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-billingconductor",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BillingConductor 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.BillingConductor 2.9.1 service generated with"
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
     keywords="aiobotocore billingconductor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_billingconductor": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/__init__.py` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListPricingRulesAssociatedToPricingPlanPaginator,
     ListPricingRulesPaginator,
     ListResourcesAssociatedToCustomLineItemPaginator,
 )
 
 Client = BillingConductorClient
 
-
 __all__ = (
     "BillingConductorClient",
     "Client",
     "ListAccountAssociationsPaginator",
     "ListBillingGroupCostReportsPaginator",
     "ListBillingGroupsPaginator",
     "ListCustomLineItemVersionsPaginator",
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/__init__.pyi` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/__main__.py` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BillingConductor 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.BillingConductor 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor\nOther"
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

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/client.py` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BillingConductorClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -150,29 +149,29 @@
         """
 
     async def batch_associate_resources_to_custom_line_item(
         self,
         *,
         TargetArn: str,
         ResourceArns: Sequence[str],
-        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...
+        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
     ) -> BatchAssociateResourcesToCustomLineItemOutputTypeDef:
         """
         Associates a batch of resources to a percentage custom line item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.batch_associate_resources_to_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#batch_associate_resources_to_custom_line_item)
         """
 
     async def batch_disassociate_resources_from_custom_line_item(
         self,
         *,
         TargetArn: str,
         ResourceArns: Sequence[str],
-        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...
+        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
     ) -> BatchDisassociateResourcesFromCustomLineItemOutputTypeDef:
         """
         Disassociates a batch of resources from a percentage custom line item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.batch_disassociate_resources_from_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#batch_disassociate_resources_from_custom_line_item)
         """
@@ -198,15 +197,15 @@
         *,
         Name: str,
         AccountGrouping: AccountGroupingTypeDef,
         ComputationPreference: ComputationPreferenceTypeDef,
         ClientToken: str = ...,
         PrimaryAccountId: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateBillingGroupOutputTypeDef:
         """
         Creates a billing group that resembles a consolidated billing family that
         Amazon Web Services charges, based off of the predefined pricing plan
         computation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.create_billing_group)
@@ -219,15 +218,15 @@
         Name: str,
         Description: str,
         BillingGroupArn: str,
         ChargeDetails: CustomLineItemChargeDetailsTypeDef,
         ClientToken: str = ...,
         BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> CreateCustomLineItemOutputTypeDef:
         """
         Creates a custom line item that can be used to create a one-time fixed charge
         that can be applied to a single billing group for the current or previous
         billing
         period.
 
@@ -238,15 +237,15 @@
     async def create_pricing_plan(
         self,
         *,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
         PricingRuleArns: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePricingPlanOutputTypeDef:
         """
         Creates a pricing plan that is used for computing Amazon Web Services charges
         for billing
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.create_pricing_plan)
@@ -263,15 +262,15 @@
         Description: str = ...,
         ModifierPercentage: float = ...,
         Service: str = ...,
         Tags: Mapping[str, str] = ...,
         BillingEntity: str = ...,
         Tiering: CreateTieringInputTypeDef = ...,
         UsageType: str = ...,
-        Operation: str = ...
+        Operation: str = ...,
     ) -> CreatePricingRuleOutputTypeDef:
         """
         Creates a pricing rule can be associated to a pricing plan, or a set of pricing
         plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.create_pricing_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#create_pricing_rule)
@@ -349,15 +348,15 @@
         """
 
     async def list_account_associations(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssociationsOutputTypeDef:
         """
         This is a paginated call to list linked accounts that are linked to the payer
         account for the specified time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_account_associations)
@@ -366,15 +365,15 @@
 
     async def list_billing_group_cost_reports(
         self,
         *,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListBillingGroupCostReportsFilterTypeDef = ...
+        Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
     ) -> ListBillingGroupCostReportsOutputTypeDef:
         """
         A paginated call to retrieve a summary report of actual Amazon Web Services
         charges and the calculated Amazon Web Services charges based on the associated
         pricing plan of a billing
         group.
 
@@ -384,15 +383,15 @@
 
     async def list_billing_groups(
         self,
         *,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListBillingGroupsFilterTypeDef = ...
+        Filters: ListBillingGroupsFilterTypeDef = ...,
     ) -> ListBillingGroupsOutputTypeDef:
         """
         A paginated call to retrieve a list of billing groups for the given billing
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_billing_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_billing_groups)
@@ -400,30 +399,30 @@
 
     async def list_custom_line_item_versions(
         self,
         *,
         Arn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListCustomLineItemVersionsFilterTypeDef = ...
+        Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
     ) -> ListCustomLineItemVersionsOutputTypeDef:
         """
         A paginated call to get a list of all custom line item versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_custom_line_item_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_custom_line_item_versions)
         """
 
     async def list_custom_line_items(
         self,
         *,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListCustomLineItemsFilterTypeDef = ...
+        Filters: ListCustomLineItemsFilterTypeDef = ...,
     ) -> ListCustomLineItemsOutputTypeDef:
         """
         A paginated call to get a list of all custom line items (FFLIs) for the given
         billing
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_custom_line_items)
@@ -432,45 +431,45 @@
 
     async def list_pricing_plans(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingPlansOutputTypeDef:
         """
         A paginated call to get pricing plans for the given billing period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_pricing_plans)
         """
 
     async def list_pricing_plans_associated_with_pricing_rule(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingPlansAssociatedWithPricingRuleOutputTypeDef:
         """
         A list of the pricing plans that are associated with a pricing rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_plans_associated_with_pricing_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_pricing_plans_associated_with_pricing_rule)
         """
 
     async def list_pricing_rules(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingRulesOutputTypeDef:
         """
         Describes a pricing rule that can be associated to a pricing plan, or set of
         pricing
         plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_rules)
@@ -479,15 +478,15 @@
 
     async def list_pricing_rules_associated_to_pricing_plan(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingRulesAssociatedToPricingPlanOutputTypeDef:
         """
         Lists the pricing rules that are associated with a pricing plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_rules_associated_to_pricing_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_pricing_rules_associated_to_pricing_plan)
         """
@@ -495,15 +494,15 @@
     async def list_resources_associated_to_custom_line_item(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...
+        Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
     ) -> ListResourcesAssociatedToCustomLineItemOutputTypeDef:
         """
         List the resources that are associated to a custom line item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_resources_associated_to_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_resources_associated_to_custom_line_item)
         """
@@ -538,15 +537,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Status: BillingGroupStatusType = ...,
         ComputationPreference: ComputationPreferenceTypeDef = ...,
         Description: str = ...,
-        AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...
+        AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...,
     ) -> UpdateBillingGroupOutputTypeDef:
         """
         This updates an existing billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_billing_group)
         """
@@ -554,15 +553,15 @@
     async def update_custom_line_item(
         self,
         *,
         Arn: str,
         Name: str = ...,
         Description: str = ...,
         ChargeDetails: UpdateCustomLineItemChargeDetailsTypeDef = ...,
-        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...
+        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
     ) -> UpdateCustomLineItemOutputTypeDef:
         """
         Update an existing custom line item in the current or previous billing period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_custom_line_item)
         """
@@ -581,15 +580,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Description: str = ...,
         Type: PricingRuleTypeType = ...,
         ModifierPercentage: float = ...,
-        Tiering: UpdateTieringInputTypeDef = ...
+        Tiering: UpdateTieringInputTypeDef = ...,
     ) -> UpdatePricingRuleOutputTypeDef:
         """
         Updates an existing pricing rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_pricing_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_pricing_rule)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/client.pyi` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -146,29 +146,29 @@
         """
 
     async def batch_associate_resources_to_custom_line_item(
         self,
         *,
         TargetArn: str,
         ResourceArns: Sequence[str],
-        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...
+        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
     ) -> BatchAssociateResourcesToCustomLineItemOutputTypeDef:
         """
         Associates a batch of resources to a percentage custom line item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.batch_associate_resources_to_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#batch_associate_resources_to_custom_line_item)
         """
 
     async def batch_disassociate_resources_from_custom_line_item(
         self,
         *,
         TargetArn: str,
         ResourceArns: Sequence[str],
-        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...
+        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
     ) -> BatchDisassociateResourcesFromCustomLineItemOutputTypeDef:
         """
         Disassociates a batch of resources from a percentage custom line item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.batch_disassociate_resources_from_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#batch_disassociate_resources_from_custom_line_item)
         """
@@ -194,15 +194,15 @@
         *,
         Name: str,
         AccountGrouping: AccountGroupingTypeDef,
         ComputationPreference: ComputationPreferenceTypeDef,
         ClientToken: str = ...,
         PrimaryAccountId: str = ...,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateBillingGroupOutputTypeDef:
         """
         Creates a billing group that resembles a consolidated billing family that
         Amazon Web Services charges, based off of the predefined pricing plan
         computation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.create_billing_group)
@@ -215,15 +215,15 @@
         Name: str,
         Description: str,
         BillingGroupArn: str,
         ChargeDetails: CustomLineItemChargeDetailsTypeDef,
         ClientToken: str = ...,
         BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> CreateCustomLineItemOutputTypeDef:
         """
         Creates a custom line item that can be used to create a one-time fixed charge
         that can be applied to a single billing group for the current or previous
         billing
         period.
 
@@ -234,15 +234,15 @@
     async def create_pricing_plan(
         self,
         *,
         Name: str,
         ClientToken: str = ...,
         Description: str = ...,
         PricingRuleArns: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePricingPlanOutputTypeDef:
         """
         Creates a pricing plan that is used for computing Amazon Web Services charges
         for billing
         groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.create_pricing_plan)
@@ -259,15 +259,15 @@
         Description: str = ...,
         ModifierPercentage: float = ...,
         Service: str = ...,
         Tags: Mapping[str, str] = ...,
         BillingEntity: str = ...,
         Tiering: CreateTieringInputTypeDef = ...,
         UsageType: str = ...,
-        Operation: str = ...
+        Operation: str = ...,
     ) -> CreatePricingRuleOutputTypeDef:
         """
         Creates a pricing rule can be associated to a pricing plan, or a set of pricing
         plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.create_pricing_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#create_pricing_rule)
@@ -345,15 +345,15 @@
         """
 
     async def list_account_associations(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAccountAssociationsOutputTypeDef:
         """
         This is a paginated call to list linked accounts that are linked to the payer
         account for the specified time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_account_associations)
@@ -362,15 +362,15 @@
 
     async def list_billing_group_cost_reports(
         self,
         *,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListBillingGroupCostReportsFilterTypeDef = ...
+        Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
     ) -> ListBillingGroupCostReportsOutputTypeDef:
         """
         A paginated call to retrieve a summary report of actual Amazon Web Services
         charges and the calculated Amazon Web Services charges based on the associated
         pricing plan of a billing
         group.
 
@@ -380,15 +380,15 @@
 
     async def list_billing_groups(
         self,
         *,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListBillingGroupsFilterTypeDef = ...
+        Filters: ListBillingGroupsFilterTypeDef = ...,
     ) -> ListBillingGroupsOutputTypeDef:
         """
         A paginated call to retrieve a list of billing groups for the given billing
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_billing_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_billing_groups)
@@ -396,30 +396,30 @@
 
     async def list_custom_line_item_versions(
         self,
         *,
         Arn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListCustomLineItemVersionsFilterTypeDef = ...
+        Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
     ) -> ListCustomLineItemVersionsOutputTypeDef:
         """
         A paginated call to get a list of all custom line item versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_custom_line_item_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_custom_line_item_versions)
         """
 
     async def list_custom_line_items(
         self,
         *,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListCustomLineItemsFilterTypeDef = ...
+        Filters: ListCustomLineItemsFilterTypeDef = ...,
     ) -> ListCustomLineItemsOutputTypeDef:
         """
         A paginated call to get a list of all custom line items (FFLIs) for the given
         billing
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_custom_line_items)
@@ -428,45 +428,45 @@
 
     async def list_pricing_plans(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingPlansOutputTypeDef:
         """
         A paginated call to get pricing plans for the given billing period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_pricing_plans)
         """
 
     async def list_pricing_plans_associated_with_pricing_rule(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingPlansAssociatedWithPricingRuleOutputTypeDef:
         """
         A list of the pricing plans that are associated with a pricing rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_plans_associated_with_pricing_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_pricing_plans_associated_with_pricing_rule)
         """
 
     async def list_pricing_rules(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingRulesOutputTypeDef:
         """
         Describes a pricing rule that can be associated to a pricing plan, or set of
         pricing
         plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_rules)
@@ -475,15 +475,15 @@
 
     async def list_pricing_rules_associated_to_pricing_plan(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPricingRulesAssociatedToPricingPlanOutputTypeDef:
         """
         Lists the pricing rules that are associated with a pricing plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_pricing_rules_associated_to_pricing_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_pricing_rules_associated_to_pricing_plan)
         """
@@ -491,15 +491,15 @@
     async def list_resources_associated_to_custom_line_item(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...
+        Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
     ) -> ListResourcesAssociatedToCustomLineItemOutputTypeDef:
         """
         List the resources that are associated to a custom line item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.list_resources_associated_to_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#list_resources_associated_to_custom_line_item)
         """
@@ -534,15 +534,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Status: BillingGroupStatusType = ...,
         ComputationPreference: ComputationPreferenceTypeDef = ...,
         Description: str = ...,
-        AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...
+        AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...,
     ) -> UpdateBillingGroupOutputTypeDef:
         """
         This updates an existing billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_billing_group)
         """
@@ -550,15 +550,15 @@
     async def update_custom_line_item(
         self,
         *,
         Arn: str,
         Name: str = ...,
         Description: str = ...,
         ChargeDetails: UpdateCustomLineItemChargeDetailsTypeDef = ...,
-        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...
+        BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,
     ) -> UpdateCustomLineItemOutputTypeDef:
         """
         Update an existing custom line item in the current or previous billing period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_custom_line_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_custom_line_item)
         """
@@ -577,15 +577,15 @@
         self,
         *,
         Arn: str,
         Name: str = ...,
         Description: str = ...,
         Type: PricingRuleTypeType = ...,
         ModifierPercentage: float = ...,
-        Tiering: UpdateTieringInputTypeDef = ...
+        Tiering: UpdateTieringInputTypeDef = ...,
     ) -> UpdatePricingRuleOutputTypeDef:
         """
         Updates an existing pricing rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_pricing_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_pricing_rule)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/literals.py` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AssociateResourceErrorReasonType",
     "BillingGroupStatusType",
     "CurrencyCodeType",
     "CustomLineItemRelationshipType",
     "CustomLineItemTypeType",
     "LineItemFilterAttributeNameType",
@@ -43,15 +42,14 @@
     "PricingRuleTypeType",
     "BillingConductorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AssociateResourceErrorReasonType = Literal[
     "ILLEGAL_CUSTOMLINEITEM",
     "INTERNAL_SERVER_EXCEPTION",
     "INVALID_ARN",
     "INVALID_BILLING_PERIOD_RANGE",
     "SERVICE_LIMIT_EXCEEDED",
 ]
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/literals.pyi` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/paginator.py` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     "ListPricingPlansPaginator",
     "ListPricingPlansAssociatedWithPricingRulePaginator",
     "ListPricingRulesPaginator",
     "ListPricingRulesAssociatedToPricingPlanPaginator",
     "ListResourcesAssociatedToCustomLineItemPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -97,15 +96,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 
@@ -116,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 
@@ -135,15 +134,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 
@@ -154,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomLineItemVersionsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 
@@ -173,15 +172,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomLineItemsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 
@@ -192,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 
@@ -211,15 +210,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 
@@ -230,15 +229,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 
@@ -249,15 +248,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 
@@ -269,13 +268,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/paginator.pyi` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 class ListBillingGroupCostReportsPaginator(AioPaginator):
@@ -112,15 +112,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 class ListBillingGroupsPaginator(AioPaginator):
@@ -130,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 class ListCustomLineItemVersionsPaginator(AioPaginator):
@@ -148,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomLineItemVersionsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 class ListCustomLineItemsPaginator(AioPaginator):
@@ -166,15 +166,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCustomLineItemsOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 class ListPricingPlansPaginator(AioPaginator):
@@ -184,15 +184,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 class ListPricingPlansAssociatedWithPricingRulePaginator(AioPaginator):
@@ -202,15 +202,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 class ListPricingRulesPaginator(AioPaginator):
@@ -220,15 +220,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 class ListPricingRulesAssociatedToPricingPlanPaginator(AioPaginator):
@@ -238,15 +238,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 class ListResourcesAssociatedToCustomLineItemPaginator(AioPaginator):
@@ -257,13 +257,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/type_defs.py` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
     "AssociateResourceErrorTypeDef",
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor/type_defs.pyi` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/PKG-INFO` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-billingconductor
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BillingConductor 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BillingConductor 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/
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
 
 <a id="types-aiobotocore-billingconductor"></a>
 
 # types-aiobotocore-billingconductor
 
 [![PyPI - types-aiobotocore-billingconductor](https://img.shields.io/pypi/v/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingConductor 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[aiobotocore.BillingConductor 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [types-aiobotocore-billingconductor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-billingconductor-2.9.0/types_aiobotocore_billingconductor.egg-info/SOURCES.txt` & `types-aiobotocore-billingconductor-2.9.1/types_aiobotocore_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

