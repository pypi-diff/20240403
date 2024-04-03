# Comparing `tmp/types-aiobotocore-payment-cryptography-data-2.9.0.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-data-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-data-2.9.0.tar", last modified: Wed Dec 13 20:00:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-data-2.9.1.tar", last modified: Thu Jan 18 01:21:27 2024, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-data-2.9.0.tar` & `types-aiobotocore-payment-cryptography-data-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:06.349346 types-aiobotocore-payment-cryptography-data-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2023-12-13 20:00:06.349346 types-aiobotocore-payment-cryptography-data-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11619 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:06.349346 types-aiobotocore-payment-cryptography-data-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2023-12-13 19:51:26.000000 types-aiobotocore-payment-cryptography-data-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:06.349346 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21019 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21018 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:27.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:06.349346 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-13 20:00:06.000000 types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.005132 types-aiobotocore-payment-cryptography-data-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-01-18 01:21:27.005132 types-aiobotocore-payment-cryptography-data-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:27.005132 types-aiobotocore-payment-cryptography-data-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.005132 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-01-18 01:13:05.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-01-18 01:13:05.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-01-18 01:13:05.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21018 2024-01-18 01:13:05.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21018 2024-01-18 01:13:05.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:04.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:27.005132 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-01-18 01:21:26.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-18 01:21:26.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:26.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:26.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:26.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-18 01:21:26.000000 types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/LICENSE` & `types-aiobotocore-payment-cryptography-data-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/PKG-INFO` & `types-aiobotocore-payment-cryptography-data-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/
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
 
 <a id="types-aiobotocore-payment-cryptography-data"></a>
 
 # types-aiobotocore-payment-cryptography-data
 
 [![PyPI - types-aiobotocore-payment-cryptography-data](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography-data)](https://pepy.tech/project/types-aiobotocore-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyDataPlane 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[aiobotocore.PaymentCryptographyDataPlane 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [types-aiobotocore-payment-cryptography-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/README.md` & `types-aiobotocore-payment-cryptography-data-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography-data)](https://pepy.tech/project/types-aiobotocore-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyDataPlane 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[aiobotocore.PaymentCryptographyDataPlane 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [types-aiobotocore-payment-cryptography-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/setup.py` & `types-aiobotocore-payment-cryptography-data-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography-data",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_payment_cryptography_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.1 service generated with"
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
         "aiobotocore payment-cryptography-data type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_payment_cryptography_data": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/__init__.py` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import PaymentCryptographyDataPlaneClient
 
 Client = PaymentCryptographyDataPlaneClient
 
-
 __all__ = ("Client", "PaymentCryptographyDataPlaneClient")
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/__init__.pyi` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/__main__.py` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/client.py` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         """
 
     async def decrypt_data(
         self,
         *,
         CipherText: str,
         DecryptionAttributes: EncryptionDecryptionAttributesTypeDef,
-        KeyIdentifier: str
+        KeyIdentifier: str,
     ) -> DecryptDataOutputTypeDef:
         """
         Decrypts ciphertext data to plaintext using symmetric, asymmetric, or DUKPT
         data encryption
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.decrypt_data)
@@ -118,15 +118,15 @@
         """
 
     async def encrypt_data(
         self,
         *,
         EncryptionAttributes: EncryptionDecryptionAttributesTypeDef,
         KeyIdentifier: str,
-        PlainText: str
+        PlainText: str,
     ) -> EncryptDataOutputTypeDef:
         """
         Encrypts plaintext data to ciphertext using symmetric, asymmetric, or DUKPT
         data encryption
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.encrypt_data)
@@ -135,15 +135,15 @@
 
     async def generate_card_validation_data(
         self,
         *,
         GenerationAttributes: CardGenerationAttributesTypeDef,
         KeyIdentifier: str,
         PrimaryAccountNumber: str,
-        ValidationDataLength: int = ...
+        ValidationDataLength: int = ...,
     ) -> GenerateCardValidationDataOutputTypeDef:
         """
         Generates card-related validation data using algorithms such as Card
         Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2),
         or Card Security Codes
         (CSC).
 
@@ -153,15 +153,15 @@
 
     async def generate_mac(
         self,
         *,
         GenerationAttributes: MacAttributesTypeDef,
         KeyIdentifier: str,
         MessageData: str,
-        MacLength: int = ...
+        MacLength: int = ...,
     ) -> GenerateMacOutputTypeDef:
         """
         Generates a Message Authentication Code (MAC) cryptogram within Amazon Web
         Services Payment
         Cryptography.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_mac)
@@ -172,15 +172,15 @@
         self,
         *,
         EncryptionKeyIdentifier: str,
         GenerationAttributes: PinGenerationAttributesTypeDef,
         GenerationKeyIdentifier: str,
         PinBlockFormat: PinBlockFormatForPinDataType,
         PrimaryAccountNumber: str,
-        PinDataLength: int = ...
+        PinDataLength: int = ...,
     ) -> GeneratePinDataOutputTypeDef:
         """
         Generates pin-related data such as PIN, PIN Verification Value (PVV), PIN
         Block, and PIN Offset during new card issuance or
         reissuance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_pin_data)
@@ -204,15 +204,15 @@
     async def re_encrypt_data(
         self,
         *,
         CipherText: str,
         IncomingEncryptionAttributes: ReEncryptionAttributesTypeDef,
         IncomingKeyIdentifier: str,
         OutgoingEncryptionAttributes: ReEncryptionAttributesTypeDef,
-        OutgoingKeyIdentifier: str
+        OutgoingKeyIdentifier: str,
     ) -> ReEncryptDataOutputTypeDef:
         """
         Re-encrypt ciphertext using DUKPT, Symmetric and Asymmetric Data Encryption
         Keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.re_encrypt_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#re_encrypt_data)
@@ -223,15 +223,15 @@
         *,
         EncryptedPinBlock: str,
         IncomingKeyIdentifier: str,
         IncomingTranslationAttributes: TranslationIsoFormatsTypeDef,
         OutgoingKeyIdentifier: str,
         OutgoingTranslationAttributes: TranslationIsoFormatsTypeDef,
         IncomingDukptAttributes: DukptDerivationAttributesTypeDef = ...,
-        OutgoingDukptAttributes: DukptDerivationAttributesTypeDef = ...
+        OutgoingDukptAttributes: DukptDerivationAttributesTypeDef = ...,
     ) -> TranslatePinDataOutputTypeDef:
         """
         Translates encrypted PIN block from and to ISO 9564 formats 0,1,3,4.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.translate_pin_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#translate_pin_data)
         """
@@ -240,15 +240,15 @@
         self,
         *,
         AuthRequestCryptogram: str,
         KeyIdentifier: str,
         MajorKeyDerivationMode: MajorKeyDerivationModeType,
         SessionKeyDerivationAttributes: SessionKeyDerivationTypeDef,
         TransactionData: str,
-        AuthResponseAttributes: CryptogramAuthResponseTypeDef = ...
+        AuthResponseAttributes: CryptogramAuthResponseTypeDef = ...,
     ) -> VerifyAuthRequestCryptogramOutputTypeDef:
         """
         Verifies Authorization Request Cryptogram (ARQC) for a EMV chip payment card
         authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_auth_request_cryptogram)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#verify_auth_request_cryptogram)
@@ -256,15 +256,15 @@
 
     async def verify_card_validation_data(
         self,
         *,
         KeyIdentifier: str,
         PrimaryAccountNumber: str,
         ValidationData: str,
-        VerificationAttributes: CardVerificationAttributesTypeDef
+        VerificationAttributes: CardVerificationAttributesTypeDef,
     ) -> VerifyCardValidationDataOutputTypeDef:
         """
         Verifies card-related validation data using algorithms such as Card
         Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2)
         and Card Security Codes
         (CSC).
 
@@ -275,15 +275,15 @@
     async def verify_mac(
         self,
         *,
         KeyIdentifier: str,
         Mac: str,
         MessageData: str,
         VerificationAttributes: MacAttributesTypeDef,
-        MacLength: int = ...
+        MacLength: int = ...,
     ) -> VerifyMacOutputTypeDef:
         """
         Verifies a Message Authentication Code (MAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_mac)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#verify_mac)
         """
@@ -294,15 +294,15 @@
         EncryptedPinBlock: str,
         EncryptionKeyIdentifier: str,
         PinBlockFormat: PinBlockFormatForPinDataType,
         PrimaryAccountNumber: str,
         VerificationAttributes: PinVerificationAttributesTypeDef,
         VerificationKeyIdentifier: str,
         DukptAttributes: DukptAttributesTypeDef = ...,
-        PinDataLength: int = ...
+        PinDataLength: int = ...,
     ) -> VerifyPinDataOutputTypeDef:
         """
         Verifies pin-related data such as PIN and PIN Offset using algorithms including
         VISA PVV and
         IBM3624.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_pin_data)
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/client.pyi` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """
 
     async def decrypt_data(
         self,
         *,
         CipherText: str,
         DecryptionAttributes: EncryptionDecryptionAttributesTypeDef,
-        KeyIdentifier: str
+        KeyIdentifier: str,
     ) -> DecryptDataOutputTypeDef:
         """
         Decrypts ciphertext data to plaintext using symmetric, asymmetric, or DUKPT
         data encryption
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.decrypt_data)
@@ -115,15 +115,15 @@
         """
 
     async def encrypt_data(
         self,
         *,
         EncryptionAttributes: EncryptionDecryptionAttributesTypeDef,
         KeyIdentifier: str,
-        PlainText: str
+        PlainText: str,
     ) -> EncryptDataOutputTypeDef:
         """
         Encrypts plaintext data to ciphertext using symmetric, asymmetric, or DUKPT
         data encryption
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.encrypt_data)
@@ -132,15 +132,15 @@
 
     async def generate_card_validation_data(
         self,
         *,
         GenerationAttributes: CardGenerationAttributesTypeDef,
         KeyIdentifier: str,
         PrimaryAccountNumber: str,
-        ValidationDataLength: int = ...
+        ValidationDataLength: int = ...,
     ) -> GenerateCardValidationDataOutputTypeDef:
         """
         Generates card-related validation data using algorithms such as Card
         Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2),
         or Card Security Codes
         (CSC).
 
@@ -150,15 +150,15 @@
 
     async def generate_mac(
         self,
         *,
         GenerationAttributes: MacAttributesTypeDef,
         KeyIdentifier: str,
         MessageData: str,
-        MacLength: int = ...
+        MacLength: int = ...,
     ) -> GenerateMacOutputTypeDef:
         """
         Generates a Message Authentication Code (MAC) cryptogram within Amazon Web
         Services Payment
         Cryptography.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_mac)
@@ -169,15 +169,15 @@
         self,
         *,
         EncryptionKeyIdentifier: str,
         GenerationAttributes: PinGenerationAttributesTypeDef,
         GenerationKeyIdentifier: str,
         PinBlockFormat: PinBlockFormatForPinDataType,
         PrimaryAccountNumber: str,
-        PinDataLength: int = ...
+        PinDataLength: int = ...,
     ) -> GeneratePinDataOutputTypeDef:
         """
         Generates pin-related data such as PIN, PIN Verification Value (PVV), PIN
         Block, and PIN Offset during new card issuance or
         reissuance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.generate_pin_data)
@@ -201,15 +201,15 @@
     async def re_encrypt_data(
         self,
         *,
         CipherText: str,
         IncomingEncryptionAttributes: ReEncryptionAttributesTypeDef,
         IncomingKeyIdentifier: str,
         OutgoingEncryptionAttributes: ReEncryptionAttributesTypeDef,
-        OutgoingKeyIdentifier: str
+        OutgoingKeyIdentifier: str,
     ) -> ReEncryptDataOutputTypeDef:
         """
         Re-encrypt ciphertext using DUKPT, Symmetric and Asymmetric Data Encryption
         Keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.re_encrypt_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#re_encrypt_data)
@@ -220,15 +220,15 @@
         *,
         EncryptedPinBlock: str,
         IncomingKeyIdentifier: str,
         IncomingTranslationAttributes: TranslationIsoFormatsTypeDef,
         OutgoingKeyIdentifier: str,
         OutgoingTranslationAttributes: TranslationIsoFormatsTypeDef,
         IncomingDukptAttributes: DukptDerivationAttributesTypeDef = ...,
-        OutgoingDukptAttributes: DukptDerivationAttributesTypeDef = ...
+        OutgoingDukptAttributes: DukptDerivationAttributesTypeDef = ...,
     ) -> TranslatePinDataOutputTypeDef:
         """
         Translates encrypted PIN block from and to ISO 9564 formats 0,1,3,4.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.translate_pin_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#translate_pin_data)
         """
@@ -237,15 +237,15 @@
         self,
         *,
         AuthRequestCryptogram: str,
         KeyIdentifier: str,
         MajorKeyDerivationMode: MajorKeyDerivationModeType,
         SessionKeyDerivationAttributes: SessionKeyDerivationTypeDef,
         TransactionData: str,
-        AuthResponseAttributes: CryptogramAuthResponseTypeDef = ...
+        AuthResponseAttributes: CryptogramAuthResponseTypeDef = ...,
     ) -> VerifyAuthRequestCryptogramOutputTypeDef:
         """
         Verifies Authorization Request Cryptogram (ARQC) for a EMV chip payment card
         authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_auth_request_cryptogram)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#verify_auth_request_cryptogram)
@@ -253,15 +253,15 @@
 
     async def verify_card_validation_data(
         self,
         *,
         KeyIdentifier: str,
         PrimaryAccountNumber: str,
         ValidationData: str,
-        VerificationAttributes: CardVerificationAttributesTypeDef
+        VerificationAttributes: CardVerificationAttributesTypeDef,
     ) -> VerifyCardValidationDataOutputTypeDef:
         """
         Verifies card-related validation data using algorithms such as Card
         Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2)
         and Card Security Codes
         (CSC).
 
@@ -272,15 +272,15 @@
     async def verify_mac(
         self,
         *,
         KeyIdentifier: str,
         Mac: str,
         MessageData: str,
         VerificationAttributes: MacAttributesTypeDef,
-        MacLength: int = ...
+        MacLength: int = ...,
     ) -> VerifyMacOutputTypeDef:
         """
         Verifies a Message Authentication Code (MAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_mac)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/client/#verify_mac)
         """
@@ -291,15 +291,15 @@
         EncryptedPinBlock: str,
         EncryptionKeyIdentifier: str,
         PinBlockFormat: PinBlockFormatForPinDataType,
         PrimaryAccountNumber: str,
         VerificationAttributes: PinVerificationAttributesTypeDef,
         VerificationKeyIdentifier: str,
         DukptAttributes: DukptAttributesTypeDef = ...,
-        PinDataLength: int = ...
+        PinDataLength: int = ...,
     ) -> VerifyPinDataOutputTypeDef:
         """
         Verifies pin-related data such as PIN and PIN Offset using algorithms including
         VISA PVV and
         IBM3624.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane.Client.verify_pin_data)
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/literals.py` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/literals.py`

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
     "DukptDerivationTypeType",
     "DukptEncryptionModeType",
     "DukptKeyVariantType",
     "EncryptionModeType",
     "MacAlgorithmType",
     "MajorKeyDerivationModeType",
@@ -31,15 +30,14 @@
     "PinBlockFormatForPinDataType",
     "SessionKeyDerivationModeType",
     "PaymentCryptographyDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 DukptDerivationTypeType = Literal["AES_128", "AES_192", "AES_256", "TDES_2KEY", "TDES_3KEY"]
 DukptEncryptionModeType = Literal["CBC", "ECB"]
 DukptKeyVariantType = Literal["BIDIRECTIONAL", "REQUEST", "RESPONSE"]
 EncryptionModeType = Literal["CBC", "CFB", "CFB1", "CFB128", "CFB64", "CFB8", "ECB", "OFB"]
 MacAlgorithmType = Literal[
     "CMAC",
     "HMAC_SHA224",
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/literals.pyi` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/type_defs.py` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AmexCardSecurityCodeVersion1TypeDef",
     "AmexCardSecurityCodeVersion2TypeDef",
     "AsymmetricEncryptionAttributesTypeDef",
     "CardHolderVerificationValueTypeDef",
     "CardVerificationValue1TypeDef",
     "CardVerificationValue2TypeDef",
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data/type_defs.pyi` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography-data
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/
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
 
 <a id="types-aiobotocore-payment-cryptography-data"></a>
 
 # types-aiobotocore-payment-cryptography-data
 
 [![PyPI - types-aiobotocore-payment-cryptography-data](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography-data)](https://pepy.tech/project/types-aiobotocore-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyDataPlane 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[aiobotocore.PaymentCryptographyDataPlane 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [types-aiobotocore-payment-cryptography-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.9.0/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-data-2.9.1/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

