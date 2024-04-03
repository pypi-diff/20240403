# Comparing `tmp/types-aiobotocore-elbv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-elbv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elbv2-2.9.0.tar", last modified: Wed Dec 13 19:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-elbv2-2.9.1.tar", last modified: Thu Jan 18 01:20:40 2024, max compression
```

## Comparing `types-aiobotocore-elbv2-2.9.0.tar` & `types-aiobotocore-elbv2-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:15.689759 types-aiobotocore-elbv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2023-12-13 19:59:15.689759 types-aiobotocore-elbv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13822 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:15.689759 types-aiobotocore-elbv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:15.689759 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43956 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    43952 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    49040 2023-12-13 19:45:52.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49039 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:50.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2023-12-13 19:45:51.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:15.689759 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2023-12-13 19:59:15.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-12-13 19:59:15.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:15.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:15.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:15.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 19:59:15.000000 types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.449344 types-aiobotocore-elbv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-01-18 01:20:40.449344 types-aiobotocore-elbv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13822 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:40.449344 types-aiobotocore-elbv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.445344 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43974 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43971 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49039 2024-01-18 01:07:47.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49039 2024-01-18 01:07:47.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-01-18 01:07:46.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:40.449344 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-01-18 01:20:40.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-18 01:20:40.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:40.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:40.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:40.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:20:40.000000 types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elbv2-2.9.0/LICENSE` & `types-aiobotocore-elbv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-elbv2-2.9.0/PKG-INFO` & `types-aiobotocore-elbv2-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elbv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
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
 
 <a id="types-aiobotocore-elbv2"></a>
 
 # types-aiobotocore-elbv2
 
 [![PyPI - types-aiobotocore-elbv2](https://img.shields.io/pypi/v/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancingv2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[aiobotocore.ElasticLoadBalancingv2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [types-aiobotocore-elbv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elbv2-2.9.0/README.md` & `types-aiobotocore-elbv2-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancingv2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[aiobotocore.ElasticLoadBalancingv2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [types-aiobotocore-elbv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elbv2-2.9.0/setup.py` & `types-aiobotocore-elbv2-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elbv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.1 service generated with"
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
     keywords="aiobotocore elbv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elbv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/__init__.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     LoadBalancersDeletedWaiter,
     TargetDeregisteredWaiter,
     TargetInServiceWaiter,
 )
 
 Client = ElasticLoadBalancingv2Client
 
-
 __all__ = (
     "Client",
     "DescribeAccountLimitsPaginator",
     "DescribeListenerCertificatesPaginator",
     "DescribeListenersPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeRulesPaginator",
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/__init__.pyi` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/__main__.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/client.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticLoadBalancingv2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -236,15 +235,15 @@
         DefaultActions: Sequence[ActionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...
+        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...,
     ) -> CreateListenerOutputTypeDef:
         """
         Creates a listener for the specified Application Load Balancer, Network Load
         Balancer, or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_listener)
@@ -258,15 +257,15 @@
         Subnets: Sequence[str] = ...,
         SubnetMappings: Sequence[SubnetMappingTypeDef] = ...,
         SecurityGroups: Sequence[str] = ...,
         Scheme: LoadBalancerSchemeEnumType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: LoadBalancerTypeEnumType = ...,
         IpAddressType: IpAddressTypeType = ...,
-        CustomerOwnedIpv4Pool: str = ...
+        CustomerOwnedIpv4Pool: str = ...,
     ) -> CreateLoadBalancerOutputTypeDef:
         """
         Creates an Application Load Balancer, Network Load Balancer, or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_load_balancer)
@@ -275,15 +274,15 @@
     async def create_rule(
         self,
         *,
         ListenerArn: str,
         Conditions: Sequence[RuleConditionTypeDef],
         Priority: int,
         Actions: Sequence[ActionTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_rule)
         """
@@ -303,15 +302,15 @@
         HealthCheckIntervalSeconds: int = ...,
         HealthCheckTimeoutSeconds: int = ...,
         HealthyThresholdCount: int = ...,
         UnhealthyThresholdCount: int = ...,
         Matcher: MatcherTypeDef = ...,
         TargetType: TargetTypeEnumType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IpAddressType: TargetGroupIpAddressTypeEnumType = ...
+        IpAddressType: TargetGroupIpAddressTypeEnumType = ...,
     ) -> CreateTargetGroupOutputTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_target_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_target_group)
         """
@@ -319,15 +318,15 @@
     async def create_trust_store(
         self,
         *,
         Name: str,
         CaCertificatesBundleS3Bucket: str,
         CaCertificatesBundleS3Key: str,
         CaCertificatesBundleS3ObjectVersion: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustStoreOutputTypeDef:
         """
         Creates a trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_trust_store)
         """
@@ -410,15 +409,15 @@
 
     async def describe_listeners(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeListenersOutputTypeDef:
         """
         Describes the specified listeners or the listeners for the specified
         Application Load Balancer, Network Load Balancer, or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_listeners)
@@ -439,45 +438,45 @@
 
     async def describe_load_balancers(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeLoadBalancersOutputTypeDef:
         """
         Describes the specified load balancers or all of your load balancers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_load_balancers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_load_balancers)
         """
 
     async def describe_rules(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeRulesOutputTypeDef:
         """
         Describes the specified rules or the rules for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_rules)
         """
 
     async def describe_ssl_policies(
         self,
         *,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        LoadBalancerType: LoadBalancerTypeEnumType = ...
+        LoadBalancerType: LoadBalancerTypeEnumType = ...,
     ) -> DescribeSSLPoliciesOutputTypeDef:
         """
         Describes the specified policies or all policies used for SSL negotiation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_ssl_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_ssl_policies)
         """
@@ -503,29 +502,29 @@
     async def describe_target_groups(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeTargetGroupsOutputTypeDef:
         """
         Describes the specified target groups or all of your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_target_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_target_groups)
         """
 
     async def describe_target_health(
         self,
         *,
         TargetGroupArn: str,
         Targets: Sequence[TargetDescriptionTypeDef] = ...,
-        Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...
+        Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,
     ) -> DescribeTargetHealthOutputTypeDef:
         """
         Describes the health of the specified targets or all of your targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_target_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_target_health)
         """
@@ -542,15 +541,15 @@
 
     async def describe_trust_store_revocations(
         self,
         *,
         TrustStoreArn: str,
         RevocationIds: Sequence[int] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeTrustStoreRevocationsOutputTypeDef:
         """
         Describes the revocation files in use by the specified trust store arn, or
         revocation
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_trust_store_revocations)
@@ -559,15 +558,15 @@
 
     async def describe_trust_stores(
         self,
         *,
         TrustStoreArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeTrustStoresOutputTypeDef:
         """
         Describes all trust stores for a given account by trust store arn’s or name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_trust_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_trust_stores)
         """
@@ -612,15 +611,15 @@
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         DefaultActions: Sequence[ActionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
-        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...
+        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...,
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_listener)
         """
@@ -638,15 +637,15 @@
         """
 
     async def modify_rule(
         self,
         *,
         RuleArn: str,
         Conditions: Sequence[RuleConditionTypeDef] = ...,
-        Actions: Sequence[ActionTypeDef] = ...
+        Actions: Sequence[ActionTypeDef] = ...,
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_rule)
         """
@@ -659,15 +658,15 @@
         HealthCheckPort: str = ...,
         HealthCheckPath: str = ...,
         HealthCheckEnabled: bool = ...,
         HealthCheckIntervalSeconds: int = ...,
         HealthCheckTimeoutSeconds: int = ...,
         HealthyThresholdCount: int = ...,
         UnhealthyThresholdCount: int = ...,
-        Matcher: MatcherTypeDef = ...
+        Matcher: MatcherTypeDef = ...,
     ) -> ModifyTargetGroupOutputTypeDef:
         """
         Modifies the health checks used when evaluating the health state of the targets
         in the specified target
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_target_group)
@@ -686,15 +685,15 @@
 
     async def modify_trust_store(
         self,
         *,
         TrustStoreArn: str,
         CaCertificatesBundleS3Bucket: str,
         CaCertificatesBundleS3Key: str,
-        CaCertificatesBundleS3ObjectVersion: str = ...
+        CaCertificatesBundleS3ObjectVersion: str = ...,
     ) -> ModifyTrustStoreOutputTypeDef:
         """
         Update the ca certificate bundle for a given trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_trust_store)
         """
@@ -763,15 +762,15 @@
         """
 
     async def set_security_groups(
         self,
         *,
         LoadBalancerArn: str,
         SecurityGroups: Sequence[str],
-        EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType = ...
+        EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType = ...,
     ) -> SetSecurityGroupsOutputTypeDef:
         """
         Associates the specified security groups with the specified Application Load
         Balancer or Network Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.set_security_groups)
@@ -780,15 +779,15 @@
 
     async def set_subnets(
         self,
         *,
         LoadBalancerArn: str,
         Subnets: Sequence[str] = ...,
         SubnetMappings: Sequence[SubnetMappingTypeDef] = ...,
-        IpAddressType: IpAddressTypeType = ...
+        IpAddressType: IpAddressTypeType = ...,
     ) -> SetSubnetsOutputTypeDef:
         """
         Enables the Availability Zones for the specified public subnets for the
         specified Application Load Balancer, Network Load Balancer or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.set_subnets)
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/client.pyi` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         DefaultActions: Sequence[ActionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...
+        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...,
     ) -> CreateListenerOutputTypeDef:
         """
         Creates a listener for the specified Application Load Balancer, Network Load
         Balancer, or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_listener)
@@ -254,15 +254,15 @@
         Subnets: Sequence[str] = ...,
         SubnetMappings: Sequence[SubnetMappingTypeDef] = ...,
         SecurityGroups: Sequence[str] = ...,
         Scheme: LoadBalancerSchemeEnumType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: LoadBalancerTypeEnumType = ...,
         IpAddressType: IpAddressTypeType = ...,
-        CustomerOwnedIpv4Pool: str = ...
+        CustomerOwnedIpv4Pool: str = ...,
     ) -> CreateLoadBalancerOutputTypeDef:
         """
         Creates an Application Load Balancer, Network Load Balancer, or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_load_balancer)
@@ -271,15 +271,15 @@
     async def create_rule(
         self,
         *,
         ListenerArn: str,
         Conditions: Sequence[RuleConditionTypeDef],
         Priority: int,
         Actions: Sequence[ActionTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_rule)
         """
@@ -299,15 +299,15 @@
         HealthCheckIntervalSeconds: int = ...,
         HealthCheckTimeoutSeconds: int = ...,
         HealthyThresholdCount: int = ...,
         UnhealthyThresholdCount: int = ...,
         Matcher: MatcherTypeDef = ...,
         TargetType: TargetTypeEnumType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IpAddressType: TargetGroupIpAddressTypeEnumType = ...
+        IpAddressType: TargetGroupIpAddressTypeEnumType = ...,
     ) -> CreateTargetGroupOutputTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_target_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_target_group)
         """
@@ -315,15 +315,15 @@
     async def create_trust_store(
         self,
         *,
         Name: str,
         CaCertificatesBundleS3Bucket: str,
         CaCertificatesBundleS3Key: str,
         CaCertificatesBundleS3ObjectVersion: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustStoreOutputTypeDef:
         """
         Creates a trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_trust_store)
         """
@@ -406,15 +406,15 @@
 
     async def describe_listeners(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeListenersOutputTypeDef:
         """
         Describes the specified listeners or the listeners for the specified
         Application Load Balancer, Network Load Balancer, or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_listeners)
@@ -435,45 +435,45 @@
 
     async def describe_load_balancers(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeLoadBalancersOutputTypeDef:
         """
         Describes the specified load balancers or all of your load balancers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_load_balancers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_load_balancers)
         """
 
     async def describe_rules(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeRulesOutputTypeDef:
         """
         Describes the specified rules or the rules for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_rules)
         """
 
     async def describe_ssl_policies(
         self,
         *,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        LoadBalancerType: LoadBalancerTypeEnumType = ...
+        LoadBalancerType: LoadBalancerTypeEnumType = ...,
     ) -> DescribeSSLPoliciesOutputTypeDef:
         """
         Describes the specified policies or all policies used for SSL negotiation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_ssl_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_ssl_policies)
         """
@@ -499,29 +499,29 @@
     async def describe_target_groups(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeTargetGroupsOutputTypeDef:
         """
         Describes the specified target groups or all of your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_target_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_target_groups)
         """
 
     async def describe_target_health(
         self,
         *,
         TargetGroupArn: str,
         Targets: Sequence[TargetDescriptionTypeDef] = ...,
-        Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...
+        Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,
     ) -> DescribeTargetHealthOutputTypeDef:
         """
         Describes the health of the specified targets or all of your targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_target_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_target_health)
         """
@@ -538,15 +538,15 @@
 
     async def describe_trust_store_revocations(
         self,
         *,
         TrustStoreArn: str,
         RevocationIds: Sequence[int] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeTrustStoreRevocationsOutputTypeDef:
         """
         Describes the revocation files in use by the specified trust store arn, or
         revocation
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_trust_store_revocations)
@@ -555,15 +555,15 @@
 
     async def describe_trust_stores(
         self,
         *,
         TrustStoreArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
-        PageSize: int = ...
+        PageSize: int = ...,
     ) -> DescribeTrustStoresOutputTypeDef:
         """
         Describes all trust stores for a given account by trust store arn’s or name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.describe_trust_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#describe_trust_stores)
         """
@@ -608,15 +608,15 @@
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         DefaultActions: Sequence[ActionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
-        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...
+        MutualAuthentication: MutualAuthenticationAttributesTypeDef = ...,
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_listener)
         """
@@ -634,15 +634,15 @@
         """
 
     async def modify_rule(
         self,
         *,
         RuleArn: str,
         Conditions: Sequence[RuleConditionTypeDef] = ...,
-        Actions: Sequence[ActionTypeDef] = ...
+        Actions: Sequence[ActionTypeDef] = ...,
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_rule)
         """
@@ -655,15 +655,15 @@
         HealthCheckPort: str = ...,
         HealthCheckPath: str = ...,
         HealthCheckEnabled: bool = ...,
         HealthCheckIntervalSeconds: int = ...,
         HealthCheckTimeoutSeconds: int = ...,
         HealthyThresholdCount: int = ...,
         UnhealthyThresholdCount: int = ...,
-        Matcher: MatcherTypeDef = ...
+        Matcher: MatcherTypeDef = ...,
     ) -> ModifyTargetGroupOutputTypeDef:
         """
         Modifies the health checks used when evaluating the health state of the targets
         in the specified target
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_target_group)
@@ -682,15 +682,15 @@
 
     async def modify_trust_store(
         self,
         *,
         TrustStoreArn: str,
         CaCertificatesBundleS3Bucket: str,
         CaCertificatesBundleS3Key: str,
-        CaCertificatesBundleS3ObjectVersion: str = ...
+        CaCertificatesBundleS3ObjectVersion: str = ...,
     ) -> ModifyTrustStoreOutputTypeDef:
         """
         Update the ca certificate bundle for a given trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_trust_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_trust_store)
         """
@@ -759,15 +759,15 @@
         """
 
     async def set_security_groups(
         self,
         *,
         LoadBalancerArn: str,
         SecurityGroups: Sequence[str],
-        EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType = ...
+        EnforceSecurityGroupInboundRulesOnPrivateLinkTraffic: EnforceSecurityGroupInboundRulesOnPrivateLinkTrafficEnumType = ...,
     ) -> SetSecurityGroupsOutputTypeDef:
         """
         Associates the specified security groups with the specified Application Load
         Balancer or Network Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.set_security_groups)
@@ -776,15 +776,15 @@
 
     async def set_subnets(
         self,
         *,
         LoadBalancerArn: str,
         Subnets: Sequence[str] = ...,
         SubnetMappings: Sequence[SubnetMappingTypeDef] = ...,
-        IpAddressType: IpAddressTypeType = ...
+        IpAddressType: IpAddressTypeType = ...,
     ) -> SetSubnetsOutputTypeDef:
         """
         Enables the Availability Zones for the specified public subnets for the
         specified Application Load Balancer, Network Load Balancer or Gateway Load
         Balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.set_subnets)
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/literals.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/literals.py`

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
     "ActionTypeEnumType",
     "AnomalyResultEnumType",
     "AuthenticateCognitoActionConditionalBehaviorEnumType",
     "AuthenticateOidcActionConditionalBehaviorEnumType",
     "DescribeAccountLimitsPaginatorName",
     "DescribeListenerCertificatesPaginatorName",
@@ -56,15 +55,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionTypeEnumType = Literal[
     "authenticate-cognito", "authenticate-oidc", "fixed-response", "forward", "redirect"
 ]
 AnomalyResultEnumType = Literal["anomalous", "normal"]
 AuthenticateCognitoActionConditionalBehaviorEnumType = Literal["allow", "authenticate", "deny"]
 AuthenticateOidcActionConditionalBehaviorEnumType = Literal["allow", "authenticate", "deny"]
 DescribeAccountLimitsPaginatorName = Literal["describe_account_limits"]
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/literals.pyi` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/paginator.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     "DescribeListenersPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeRulesPaginator",
     "DescribeSSLPoliciesPaginator",
     "DescribeTargetGroupsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -108,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeListenersOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenerspaginator)
         """
 
 
@@ -127,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
 
@@ -146,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRulesOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describerulespaginator)
         """
 
 
@@ -165,15 +164,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describesslpoliciespaginator)
         """
 
 
@@ -185,13 +184,13 @@
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/paginator.pyi` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeListenersOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenerspaginator)
         """
 
 class DescribeLoadBalancersPaginator(AioPaginator):
@@ -121,15 +121,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
 class DescribeRulesPaginator(AioPaginator):
@@ -139,15 +139,15 @@
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRulesOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describerulespaginator)
         """
 
 class DescribeSSLPoliciesPaginator(AioPaginator):
@@ -157,15 +157,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describesslpoliciespaginator)
         """
 
 class DescribeTargetGroupsPaginator(AioPaginator):
@@ -176,13 +176,13 @@
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/type_defs.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthenticateCognitoActionConfigPaginatorTypeDef",
     "AuthenticateOidcActionConfigPaginatorTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/type_defs.pyi` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/waiter.py` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     async def wait(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.LoadBalancerAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#loadbalanceravailablewaiter)
         """
 
 
@@ -75,15 +75,15 @@
     async def wait(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.LoadBalancerExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#loadbalancerexistswaiter)
         """
 
 
@@ -96,15 +96,15 @@
     async def wait(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.LoadBalancersDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#loadbalancersdeletedwaiter)
         """
 
 
@@ -116,15 +116,15 @@
 
     async def wait(
         self,
         *,
         TargetGroupArn: str,
         Targets: Sequence[TargetDescriptionTypeDef] = ...,
         Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.TargetDeregistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#targetderegisteredwaiter)
         """
 
 
@@ -136,13 +136,13 @@
 
     async def wait(
         self,
         *,
         TargetGroupArn: str,
         Targets: Sequence[TargetDescriptionTypeDef] = ...,
         Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.TargetInService.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#targetinservicewaiter)
         """
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2/waiter.pyi` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     async def wait(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.LoadBalancerAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#loadbalanceravailablewaiter)
         """
 
 class LoadBalancerExistsWaiter(AIOWaiter):
@@ -73,15 +73,15 @@
     async def wait(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.LoadBalancerExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#loadbalancerexistswaiter)
         """
 
 class LoadBalancersDeletedWaiter(AIOWaiter):
@@ -93,15 +93,15 @@
     async def wait(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
         Marker: str = ...,
         PageSize: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.LoadBalancersDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#loadbalancersdeletedwaiter)
         """
 
 class TargetDeregisteredWaiter(AIOWaiter):
@@ -112,15 +112,15 @@
 
     async def wait(
         self,
         *,
         TargetGroupArn: str,
         Targets: Sequence[TargetDescriptionTypeDef] = ...,
         Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.TargetDeregistered.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#targetderegisteredwaiter)
         """
 
 class TargetInServiceWaiter(AIOWaiter):
@@ -131,13 +131,13 @@
 
     async def wait(
         self,
         *,
         TargetGroupArn: str,
         Targets: Sequence[TargetDescriptionTypeDef] = ...,
         Include: Sequence[DescribeTargetHealthInputIncludeEnumType] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Waiter.TargetInService.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/waiters/#targetinservicewaiter)
         """
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/PKG-INFO` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elbv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
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
 
 <a id="types-aiobotocore-elbv2"></a>
 
 # types-aiobotocore-elbv2
 
 [![PyPI - types-aiobotocore-elbv2](https://img.shields.io/pypi/v/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancingv2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[aiobotocore.ElasticLoadBalancingv2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [types-aiobotocore-elbv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elbv2-2.9.0/types_aiobotocore_elbv2.egg-info/SOURCES.txt` & `types-aiobotocore-elbv2-2.9.1/types_aiobotocore_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

