# Comparing `tmp/types-aiobotocore-payment-cryptography-2.9.0.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-2.9.0.tar", last modified: Wed Dec 13 20:00:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-2.9.1.tar", last modified: Thu Jan 18 01:21:27 2024, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-2.9.0.tar` & `types-aiobotocore-payment-cryptography-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:06.725343 types-aiobotocore-payment-cryptography-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14069 2023-12-13 20:00:06.725343 types-aiobotocore-payment-cryptography-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:06.725343 types-aiobotocore-payment-cryptography-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:06.725343 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20020 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20016 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10395 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:06.725343 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14069 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.337130 types-aiobotocore-payment-cryptography-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-01-18 01:21:27.337130 types-aiobotocore-payment-cryptography-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:27.337130 types-aiobotocore-payment-cryptography-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.337130 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20022 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20019 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.337130 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-01-18 01:21:27.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-18 01:21:27.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:27.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:27.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:27.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 01:21:27.000000 types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/LICENSE` & `types-aiobotocore-payment-cryptography-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
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
 
 <a id="types-aiobotocore-payment-cryptography"></a>
 
 # types-aiobotocore-payment-cryptography
 
 [![PyPI - types-aiobotocore-payment-cryptography](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography)](https://pepy.tech/project/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [types-aiobotocore-payment-cryptography docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/README.md` & `types-aiobotocore-payment-cryptography-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography)](https://pepy.tech/project/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [types-aiobotocore-payment-cryptography docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/setup.py` & `types-aiobotocore-payment-cryptography-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.0 service generated"
-        " with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.1 service generated"
+        " with mypy-boto3-builder 7.23.1"
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
         "aiobotocore payment-cryptography type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_payment_cryptography": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/__init__.py` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import PaymentCryptographyControlPlaneClient
 from .paginator import ListAliasesPaginator, ListKeysPaginator, ListTagsForResourcePaginator
 
 Client = PaymentCryptographyControlPlaneClient
 
-
 __all__ = (
     "Client",
     "ListAliasesPaginator",
     "ListKeysPaginator",
     "ListTagsForResourcePaginator",
     "PaymentCryptographyControlPlaneClient",
 )
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/__init__.pyi` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/__main__.py` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/client.py` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PaymentCryptographyControlPlaneClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -128,15 +127,15 @@
     async def create_key(
         self,
         *,
         Exportable: bool,
         KeyAttributes: KeyAttributesTypeDef,
         Enabled: bool = ...,
         KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateKeyOutputTypeDef:
         """
         Creates an Amazon Web Services Payment Cryptography key, a logical
         representation of a cryptographic key, that is unique in your account and
         Amazon Web Services
         Region.
 
@@ -165,15 +164,15 @@
         """
 
     async def export_key(
         self,
         *,
         ExportKeyIdentifier: str,
         KeyMaterial: ExportKeyMaterialTypeDef,
-        ExportAttributes: ExportAttributesTypeDef = ...
+        ExportAttributes: ExportAttributesTypeDef = ...,
     ) -> ExportKeyOutputTypeDef:
         """
         Exports a key from Amazon Web Services Payment Cryptography.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client.export_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/client/#export_key)
         """
@@ -248,15 +247,15 @@
 
     async def import_key(
         self,
         *,
         KeyMaterial: ImportKeyMaterialTypeDef,
         Enabled: bool = ...,
         KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportKeyOutputTypeDef:
         """
         Imports symmetric keys and public key certificates in PEM format (base64
         encoded) into Amazon Web Services Payment
         Cryptography.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client.import_key)
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/client.pyi` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     async def create_key(
         self,
         *,
         Exportable: bool,
         KeyAttributes: KeyAttributesTypeDef,
         Enabled: bool = ...,
         KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateKeyOutputTypeDef:
         """
         Creates an Amazon Web Services Payment Cryptography key, a logical
         representation of a cryptographic key, that is unique in your account and
         Amazon Web Services
         Region.
 
@@ -161,15 +161,15 @@
         """
 
     async def export_key(
         self,
         *,
         ExportKeyIdentifier: str,
         KeyMaterial: ExportKeyMaterialTypeDef,
-        ExportAttributes: ExportAttributesTypeDef = ...
+        ExportAttributes: ExportAttributesTypeDef = ...,
     ) -> ExportKeyOutputTypeDef:
         """
         Exports a key from Amazon Web Services Payment Cryptography.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client.export_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/client/#export_key)
         """
@@ -244,15 +244,15 @@
 
     async def import_key(
         self,
         *,
         KeyMaterial: ImportKeyMaterialTypeDef,
         Enabled: bool = ...,
         KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportKeyOutputTypeDef:
         """
         Imports symmetric keys and public key certificates in PEM format (base64
         encoded) into Amazon Web Services Payment
         Cryptography.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client.import_key)
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/literals.py` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/literals.py`

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
     "KeyAlgorithmType",
     "KeyCheckValueAlgorithmType",
     "KeyClassType",
     "KeyMaterialTypeType",
     "KeyOriginType",
     "KeyStateType",
@@ -35,15 +34,14 @@
     "WrappedKeyMaterialFormatType",
     "PaymentCryptographyControlPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 KeyAlgorithmType = Literal[
     "AES_128", "AES_192", "AES_256", "RSA_2048", "RSA_3072", "RSA_4096", "TDES_2KEY", "TDES_3KEY"
 ]
 KeyCheckValueAlgorithmType = Literal["ANSI_X9_24", "CMAC"]
 KeyClassType = Literal["ASYMMETRIC_KEY_PAIR", "PRIVATE_KEY", "PUBLIC_KEY", "SYMMETRIC_KEY"]
 KeyMaterialTypeType = Literal[
     "ROOT_PUBLIC_KEY_CERTIFICATE",
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/literals.pyi` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/paginator.py` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListKeysOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAliasesPaginator", "ListKeysPaginator", "ListTagsForResourcePaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/paginator.pyi` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/type_defs.py` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography/type_defs.pyi` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
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
 
 <a id="types-aiobotocore-payment-cryptography"></a>
 
 # types-aiobotocore-payment-cryptography
 
 [![PyPI - types-aiobotocore-payment-cryptography](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography)](https://pepy.tech/project/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [types-aiobotocore-payment-cryptography docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-payment-cryptography-2.9.0/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-2.9.1/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

