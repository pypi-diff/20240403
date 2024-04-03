# Comparing `tmp/types-aiobotocore-route53-recovery-readiness-2.9.0.tar.gz` & `tmp/types-aiobotocore-route53-recovery-readiness-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.9.0.tar", last modified: Wed Dec 13 20:00:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.9.1.tar", last modified: Thu Jan 18 01:21:40 2024, max compression
```

## Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0.tar` & `types-aiobotocore-route53-recovery-readiness-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.121218 types-aiobotocore-route53-recovery-readiness-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15647 2023-12-13 20:00:21.121218 types-aiobotocore-route53-recovery-readiness-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14010 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:21.121218 types-aiobotocore-route53-recovery-readiness-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.117218 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30696 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30692 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13797 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24703 2023-12-13 19:54:53.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24702 2023-12-13 19:54:53.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:52.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.121218 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15647 2023-12-13 20:00:21.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 20:00:21.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:21.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:21.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:21.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-13 20:00:21.000000 types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.373073 types-aiobotocore-route53-recovery-readiness-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-01-18 01:21:40.373073 types-aiobotocore-route53-recovery-readiness-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:40.373073 types-aiobotocore-route53-recovery-readiness-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.373073 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30697 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-01-18 01:16:29.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:28.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.373073 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-18 01:21:40.000000 types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/LICENSE` & `types-aiobotocore-route53-recovery-readiness-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/PKG-INFO` & `types-aiobotocore-route53-recovery-readiness-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-readiness
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/
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
 
 <a id="types-aiobotocore-route53-recovery-readiness"></a>
 
 # types-aiobotocore-route53-recovery-readiness
 
 [![PyPI - types-aiobotocore-route53-recovery-readiness](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-readiness)](https://pepy.tech/project/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [types-aiobotocore-route53-recovery-readiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/README.md` & `types-aiobotocore-route53-recovery-readiness-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-readiness)](https://pepy.tech/project/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [types-aiobotocore-route53-recovery-readiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/setup.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-readiness",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.1 service generated with"
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
         "aiobotocore route53-recovery-readiness type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53_recovery_readiness": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/__init__.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListRecoveryGroupsPaginator,
     ListResourceSetsPaginator,
     ListRulesPaginator,
 )
 
 Client = Route53RecoveryReadinessClient
 
-
 __all__ = (
     "Client",
     "GetCellReadinessSummaryPaginator",
     "GetReadinessCheckResourceStatusPaginator",
     "GetReadinessCheckStatusPaginator",
     "GetRecoveryGroupReadinessSummaryPaginator",
     "ListCellsPaginator",
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/__init__.pyi` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/__main__.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/client.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53RecoveryReadinessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -165,15 +164,15 @@
 
     async def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
         Resources: Sequence[ResourceTypeDef],
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#create_resource_set)
         """
@@ -283,15 +282,15 @@
 
     async def get_readiness_check_resource_status(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetReadinessCheckResourceStatusResponseTypeDef:
         """
         Gets individual readiness status for a readiness check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_readiness_check_resource_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#get_readiness_check_resource_status)
         """
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/client.pyi` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
     async def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
         Resources: Sequence[ResourceTypeDef],
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#create_resource_set)
         """
@@ -279,15 +279,15 @@
 
     async def get_readiness_check_resource_status(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetReadinessCheckResourceStatusResponseTypeDef:
         """
         Gets individual readiness status for a readiness check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_readiness_check_resource_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#get_readiness_check_resource_status)
         """
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/literals.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/literals.py`

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
     "GetCellReadinessSummaryPaginatorName",
     "GetReadinessCheckResourceStatusPaginatorName",
     "GetReadinessCheckStatusPaginatorName",
     "GetRecoveryGroupReadinessSummaryPaginatorName",
     "ListCellsPaginatorName",
     "ListCrossAccountAuthorizationsPaginatorName",
@@ -34,15 +33,14 @@
     "ReadinessType",
     "Route53RecoveryReadinessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 GetCellReadinessSummaryPaginatorName = Literal["get_cell_readiness_summary"]
 GetReadinessCheckResourceStatusPaginatorName = Literal["get_readiness_check_resource_status"]
 GetReadinessCheckStatusPaginatorName = Literal["get_readiness_check_status"]
 GetRecoveryGroupReadinessSummaryPaginatorName = Literal["get_recovery_group_readiness_summary"]
 ListCellsPaginatorName = Literal["list_cells"]
 ListCrossAccountAuthorizationsPaginatorName = Literal["list_cross_account_authorizations"]
 ListReadinessChecksPaginatorName = Literal["list_readiness_checks"]
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/literals.pyi` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/paginator.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     "ListCrossAccountAuthorizationsPaginator",
     "ListReadinessChecksPaginator",
     "ListRecoveryGroupsPaginator",
     "ListResourceSetsPaginator",
     "ListRulesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -104,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetReadinessCheckResourceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckResourceStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/paginators/#getreadinesscheckresourcestatuspaginator)
         """
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/paginator.pyi` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         ReadinessCheckName: str,
         ResourceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetReadinessCheckResourceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Paginator.GetReadinessCheckResourceStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/paginators/#getreadinesscheckresourcestatuspaginator)
         """
 
 class GetReadinessCheckStatusPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/type_defs.py` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/type_defs.py`

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
     "CellOutputTypeDef",
     "CreateCellRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateCrossAccountAuthorizationRequestRequestTypeDef",
     "CreateReadinessCheckRequestRequestTypeDef",
     "CreateRecoveryGroupRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness/type_defs.pyi` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-readiness
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/
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
 
 <a id="types-aiobotocore-route53-recovery-readiness"></a>
 
 # types-aiobotocore-route53-recovery-readiness
 
 [![PyPI - types-aiobotocore-route53-recovery-readiness](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-readiness)](https://pepy.tech/project/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [types-aiobotocore-route53-recovery-readiness docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.9.0/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-readiness-2.9.1/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

