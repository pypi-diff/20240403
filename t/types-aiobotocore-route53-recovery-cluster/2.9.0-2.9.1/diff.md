# Comparing `tmp/types-aiobotocore-route53-recovery-cluster-2.9.0.tar.gz` & `tmp/types-aiobotocore-route53-recovery-cluster-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-cluster-2.9.0.tar", last modified: Wed Dec 13 20:00:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-cluster-2.9.1.tar", last modified: Thu Jan 18 01:21:39 2024, max compression
```

## Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0.tar` & `types-aiobotocore-route53-recovery-cluster-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:20.377224 types-aiobotocore-route53-recovery-cluster-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2023-12-13 20:00:20.377224 types-aiobotocore-route53-recovery-cluster-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:20.377224 types-aiobotocore-route53-recovery-cluster-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:20.373224 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-12-13 19:54:51.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:50.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:20.377224 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-13 20:00:20.000000 types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.709076 types-aiobotocore-route53-recovery-cluster-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-01-18 01:21:39.705076 types-aiobotocore-route53-recovery-cluster-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:39.709076 types-aiobotocore-route53-recovery-cluster-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.705076 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-01-18 01:16:24.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-01-18 01:16:24.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:23.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.705076 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-01-18 01:21:39.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-18 01:21:39.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:39.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:39.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:39.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-18 01:21:39.000000 types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/LICENSE` & `types-aiobotocore-route53-recovery-cluster-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/PKG-INFO` & `types-aiobotocore-route53-recovery-cluster-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-cluster
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/
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
 
 <a id="types-aiobotocore-route53-recovery-cluster"></a>
 
 # types-aiobotocore-route53-recovery-cluster
 
 [![PyPI - types-aiobotocore-route53-recovery-cluster](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-cluster)](https://pepy.tech/project/types-aiobotocore-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryCluster 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[aiobotocore.Route53RecoveryCluster 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/README.md` & `types-aiobotocore-route53-recovery-cluster-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-cluster)](https://pepy.tech/project/types-aiobotocore-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryCluster 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[aiobotocore.Route53RecoveryCluster 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/setup.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-cluster",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_route53_recovery_cluster"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53RecoveryCluster 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Route53RecoveryCluster 2.9.1 service generated with"
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
         "aiobotocore route53-recovery-cluster type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53_recovery_cluster": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/__init__.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import Route53RecoveryClusterClient
 from .paginator import ListRoutingControlsPaginator
 
 Client = Route53RecoveryClusterClient
 
-
 __all__ = ("Client", "ListRoutingControlsPaginator", "Route53RecoveryClusterClient")
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/__init__.pyi` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/__main__.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53RecoveryCluster 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Route53RecoveryCluster 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/client.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,38 +30,34 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53RecoveryClusterClient",)
 
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
     ConflictException: Type[BotocoreClientError]
     EndpointTemporarilyUnavailableException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class Route53RecoveryClusterClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/client/)
     """
 
     meta: ClientMeta
@@ -129,28 +125,28 @@
         """
 
     async def update_routing_control_state(
         self,
         *,
         RoutingControlArn: str,
         RoutingControlState: RoutingControlStateType,
-        SafetyRulesToOverride: Sequence[str] = ...
+        SafetyRulesToOverride: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Set the state of the routing control to reroute traffic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/client/#update_routing_control_state)
         """
 
     async def update_routing_control_states(
         self,
         *,
         UpdateRoutingControlStateEntries: Sequence[UpdateRoutingControlStateEntryTypeDef],
-        SafetyRulesToOverride: Sequence[str] = ...
+        SafetyRulesToOverride: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Set multiple routing control states.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_states)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/client/#update_routing_control_states)
         """
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/client.pyi` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,32 +32,35 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("Route53RecoveryClusterClient",)
 
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
     ConflictException: Type[BotocoreClientError]
     EndpointTemporarilyUnavailableException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class Route53RecoveryClusterClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/client/)
     """
 
     meta: ClientMeta
@@ -125,28 +128,28 @@
         """
 
     async def update_routing_control_state(
         self,
         *,
         RoutingControlArn: str,
         RoutingControlState: RoutingControlStateType,
-        SafetyRulesToOverride: Sequence[str] = ...
+        SafetyRulesToOverride: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Set the state of the routing control to reroute traffic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/client/#update_routing_control_state)
         """
 
     async def update_routing_control_states(
         self,
         *,
         UpdateRoutingControlStateEntries: Sequence[UpdateRoutingControlStateEntryTypeDef],
-        SafetyRulesToOverride: Sequence[str] = ...
+        SafetyRulesToOverride: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Set multiple routing control states.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_states)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/client/#update_routing_control_states)
         """
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/literals.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListRoutingControlsPaginatorName",
     "RoutingControlStateType",
     "Route53RecoveryClusterServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListRoutingControlsPaginatorName = Literal["list_routing_controls"]
 RoutingControlStateType = Literal["Off", "On"]
 Route53RecoveryClusterServiceName = Literal["route53-recovery-cluster"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/literals.pyi` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/paginator.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListRoutingControlsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListRoutingControlsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/paginator.pyi` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/type_defs.py` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/type_defs.py`

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
     "GetRoutingControlStateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster/type_defs.pyi` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-cluster
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/
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
 
 <a id="types-aiobotocore-route53-recovery-cluster"></a>
 
 # types-aiobotocore-route53-recovery-cluster
 
 [![PyPI - types-aiobotocore-route53-recovery-cluster](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-cluster)](https://pepy.tech/project/types-aiobotocore-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryCluster 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[aiobotocore.Route53RecoveryCluster 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.9.0/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-cluster-2.9.1/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

