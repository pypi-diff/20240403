# Comparing `tmp/types-aiobotocore-acm-pca-2.9.0.tar.gz` & `tmp/types-aiobotocore-acm-pca-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-pca-2.9.0.tar", last modified: Wed Dec 13 19:58:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-pca-2.9.1.tar", last modified: Thu Jan 18 01:19:58 2024, max compression
```

## Comparing `types-aiobotocore-acm-pca-2.9.0.tar` & `types-aiobotocore-acm-pca-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.754136 types-aiobotocore-acm-pca-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-13 19:58:29.750136 types-aiobotocore-acm-pca-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:29.754136 types-aiobotocore-acm-pca-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.750136 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23932 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23928 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11807 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11805 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25155 2023-12-13 19:40:37.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25154 2023-12-13 19:40:37.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2023-12-13 19:40:36.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.750136 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-13 19:58:29.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 19:58:29.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:29.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:29.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:29.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:29.000000 types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.273537 types-aiobotocore-acm-pca-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-01-18 01:19:58.273537 types-aiobotocore-acm-pca-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:58.273537 types-aiobotocore-acm-pca-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.273537 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23938 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23935 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-01-18 01:02:37.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-18 01:02:36.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:58.273537 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-01-18 01:19:58.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-18 01:19:58.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:58.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:58.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:58.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:19:58.000000 types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/LICENSE` & `types-aiobotocore-acm-pca-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-acm-pca-2.9.0/PKG-INFO` & `types-aiobotocore-acm-pca-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm-pca
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ACMPCA 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ACMPCA 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/
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
 
 <a id="types-aiobotocore-acm-pca"></a>
 
 # types-aiobotocore-acm-pca
 
 [![PyPI - types-aiobotocore-acm-pca](https://img.shields.io/pypi/v/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm-pca)](https://pepy.tech/project/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACMPCA 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[aiobotocore.ACMPCA 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [types-aiobotocore-acm-pca docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/README.md` & `types-aiobotocore-acm-pca-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm-pca)](https://pepy.tech/project/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACMPCA 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[aiobotocore.ACMPCA 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [types-aiobotocore-acm-pca docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/setup.py` & `types-aiobotocore-acm-pca-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm-pca",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ACMPCA 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.ACMPCA 2.9.1 service generated with mypy-boto3-builder"
+        " 7.23.1"
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
     keywords="aiobotocore acm-pca type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_acm_pca": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/__init__.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     AuditReportCreatedWaiter,
     CertificateAuthorityCSRCreatedWaiter,
     CertificateIssuedWaiter,
 )
 
 Client = ACMPCAClient
 
-
 __all__ = (
     "ACMPCAClient",
     "AuditReportCreatedWaiter",
     "CertificateAuthorityCSRCreatedWaiter",
     "CertificateIssuedWaiter",
     "Client",
     "ListCertificateAuthoritiesPaginator",
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/__init__.pyi` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/__main__.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACMPCA 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ACMPCA 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/client.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ACMPCAClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -142,44 +141,44 @@
         *,
         CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UsageMode: CertificateAuthorityUsageModeType = ...
+        UsageMode: CertificateAuthorityUsageModeType = ...,
     ) -> CreateCertificateAuthorityResponseTypeDef:
         """
         Creates a root or subordinate private certificate authority (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_certificate_authority)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#create_certificate_authority)
         """
 
     async def create_certificate_authority_audit_report(
         self,
         *,
         CertificateAuthorityArn: str,
         S3BucketName: str,
-        AuditReportResponseFormat: AuditReportResponseFormatType
+        AuditReportResponseFormat: AuditReportResponseFormatType,
     ) -> CreateCertificateAuthorityAuditReportResponseTypeDef:
         """
         Creates an audit report that lists every time that your CA private key is used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_certificate_authority_audit_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#create_certificate_authority_audit_report)
         """
 
     async def create_permission(
         self,
         *,
         CertificateAuthorityArn: str,
         Principal: str,
         Actions: Sequence[ActionTypeType],
-        SourceAccount: str = ...
+        SourceAccount: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Grants one or more permissions on a private CA to the Certificate Manager (ACM)
         service principal (
         `acm.amazonaws.com`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_permission)
@@ -298,15 +297,15 @@
         """
 
     async def import_certificate_authority_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
         Certificate: BlobTypeDef,
-        CertificateChain: BlobTypeDef = ...
+        CertificateChain: BlobTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Imports a signed private CA certificate into Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.import_certificate_authority_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#import_certificate_authority_certificate)
         """
@@ -317,15 +316,15 @@
         CertificateAuthorityArn: str,
         Csr: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmType,
         Validity: ValidityTypeDef,
         ApiPassthrough: ApiPassthroughTypeDef = ...,
         TemplateArn: str = ...,
         ValidityNotBefore: ValidityTypeDef = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> IssueCertificateResponseTypeDef:
         """
         Uses your private certificate authority (CA), or one that has been shared with
         you, to issue a client
         certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.issue_certificate)
@@ -387,15 +386,15 @@
         """
 
     async def revoke_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
         CertificateSerial: str,
-        RevocationReason: RevocationReasonType
+        RevocationReason: RevocationReasonType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Revokes a certificate that was issued inside Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.revoke_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#revoke_certificate)
         """
@@ -421,15 +420,15 @@
         """
 
     async def update_certificate_authority(
         self,
         *,
         CertificateAuthorityArn: str,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
-        Status: CertificateAuthorityStatusType = ...
+        Status: CertificateAuthorityStatusType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the status or configuration of a private certificate authority (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.update_certificate_authority)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#update_certificate_authority)
         """
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/client.pyi` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -138,44 +138,44 @@
         *,
         CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UsageMode: CertificateAuthorityUsageModeType = ...
+        UsageMode: CertificateAuthorityUsageModeType = ...,
     ) -> CreateCertificateAuthorityResponseTypeDef:
         """
         Creates a root or subordinate private certificate authority (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_certificate_authority)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#create_certificate_authority)
         """
 
     async def create_certificate_authority_audit_report(
         self,
         *,
         CertificateAuthorityArn: str,
         S3BucketName: str,
-        AuditReportResponseFormat: AuditReportResponseFormatType
+        AuditReportResponseFormat: AuditReportResponseFormatType,
     ) -> CreateCertificateAuthorityAuditReportResponseTypeDef:
         """
         Creates an audit report that lists every time that your CA private key is used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_certificate_authority_audit_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#create_certificate_authority_audit_report)
         """
 
     async def create_permission(
         self,
         *,
         CertificateAuthorityArn: str,
         Principal: str,
         Actions: Sequence[ActionTypeType],
-        SourceAccount: str = ...
+        SourceAccount: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Grants one or more permissions on a private CA to the Certificate Manager (ACM)
         service principal (
         `acm.amazonaws.com`).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.create_permission)
@@ -294,15 +294,15 @@
         """
 
     async def import_certificate_authority_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
         Certificate: BlobTypeDef,
-        CertificateChain: BlobTypeDef = ...
+        CertificateChain: BlobTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Imports a signed private CA certificate into Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.import_certificate_authority_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#import_certificate_authority_certificate)
         """
@@ -313,15 +313,15 @@
         CertificateAuthorityArn: str,
         Csr: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmType,
         Validity: ValidityTypeDef,
         ApiPassthrough: ApiPassthroughTypeDef = ...,
         TemplateArn: str = ...,
         ValidityNotBefore: ValidityTypeDef = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> IssueCertificateResponseTypeDef:
         """
         Uses your private certificate authority (CA), or one that has been shared with
         you, to issue a client
         certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.issue_certificate)
@@ -383,15 +383,15 @@
         """
 
     async def revoke_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
         CertificateSerial: str,
-        RevocationReason: RevocationReasonType
+        RevocationReason: RevocationReasonType,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Revokes a certificate that was issued inside Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.revoke_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#revoke_certificate)
         """
@@ -417,15 +417,15 @@
         """
 
     async def update_certificate_authority(
         self,
         *,
         CertificateAuthorityArn: str,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
-        Status: CertificateAuthorityStatusType = ...
+        Status: CertificateAuthorityStatusType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the status or configuration of a private certificate authority (CA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.update_certificate_authority)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#update_certificate_authority)
         """
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/literals.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/literals.py`

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
     "AccessMethodTypeType",
     "ActionTypeType",
     "AuditReportCreatedWaiterName",
     "AuditReportResponseFormatType",
     "AuditReportStatusType",
     "CertificateAuthorityCSRCreatedWaiterName",
@@ -48,15 +47,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AccessMethodTypeType = Literal["CA_REPOSITORY", "RESOURCE_PKI_MANIFEST", "RESOURCE_PKI_NOTIFY"]
 ActionTypeType = Literal["GetCertificate", "IssueCertificate", "ListPermissions"]
 AuditReportCreatedWaiterName = Literal["audit_report_created"]
 AuditReportResponseFormatType = Literal["CSV", "JSON"]
 AuditReportStatusType = Literal["CREATING", "FAILED", "SUCCESS"]
 CertificateAuthorityCSRCreatedWaiterName = Literal["certificate_authority_csr_created"]
 CertificateAuthorityStatusType = Literal[
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/literals.pyi` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/paginator.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListPermissionsResponseTypeDef,
     ListTagsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListCertificateAuthoritiesPaginator", "ListPermissionsPaginator", "ListTagsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -57,15 +56,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/paginators/#listcertificateauthoritiespaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceOwner: ResourceOwnerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCertificateAuthoritiesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/paginators/#listcertificateauthoritiespaginator)
         """
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/paginator.pyi` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/paginators/#listcertificateauthoritiespaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceOwner: ResourceOwnerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCertificateAuthoritiesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/paginators/#listcertificateauthoritiespaginator)
         """
 
 class ListPermissionsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/type_defs.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/type_defs.py`

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
     "CustomAttributeTypeDef",
     "AccessMethodTypeDef",
     "BlobTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/type_defs.pyi` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/waiter.py` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
 
     async def wait(
         self,
         *,
         CertificateAuthorityArn: str,
         AuditReportId: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Waiter.AuditReportCreated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/waiters/#auditreportcreatedwaiter)
         """
 
 
@@ -77,13 +77,13 @@
     """
 
     async def wait(
         self,
         *,
         CertificateAuthorityArn: str,
         CertificateArn: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Waiter.CertificateIssued.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/waiters/#certificateissuedwaiter)
         """
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca/waiter.pyi` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """
 
     async def wait(
         self,
         *,
         CertificateAuthorityArn: str,
         AuditReportId: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Waiter.AuditReportCreated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/waiters/#auditreportcreatedwaiter)
         """
 
 class CertificateAuthorityCSRCreatedWaiter(AIOWaiter):
@@ -74,13 +74,13 @@
     """
 
     async def wait(
         self,
         *,
         CertificateAuthorityArn: str,
         CertificateArn: str,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Waiter.CertificateIssued.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/waiters/#certificateissuedwaiter)
         """
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/PKG-INFO` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm-pca
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ACMPCA 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ACMPCA 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/
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
 
 <a id="types-aiobotocore-acm-pca"></a>
 
 # types-aiobotocore-acm-pca
 
 [![PyPI - types-aiobotocore-acm-pca](https://img.shields.io/pypi/v/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm-pca)](https://pepy.tech/project/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACMPCA 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[aiobotocore.ACMPCA 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [types-aiobotocore-acm-pca docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-acm-pca-2.9.0/types_aiobotocore_acm_pca.egg-info/SOURCES.txt` & `types-aiobotocore-acm-pca-2.9.1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

