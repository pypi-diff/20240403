# Comparing `tmp/types-aiobotocore-ssm-sap-2.9.0.tar.gz` & `tmp/types-aiobotocore-ssm-sap-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-sap-2.9.0.tar", last modified: Wed Dec 13 20:00:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-sap-2.9.1.tar", last modified: Thu Jan 18 01:21:54 2024, max compression
```

## Comparing `types-aiobotocore-ssm-sap-2.9.0.tar` & `types-aiobotocore-ssm-sap-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:36.309088 types-aiobotocore-ssm-sap-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2023-12-13 20:00:36.309088 types-aiobotocore-ssm-sap-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:36.313088 types-aiobotocore-ssm-sap-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:36.309088 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17375 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17371 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2023-12-13 19:57:00.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2023-12-13 19:56:57.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2023-12-13 19:57:00.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17396 2023-12-13 19:57:00.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:56.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:36.309088 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2023-12-13 20:00:36.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 20:00:36.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:36.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:36.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:36.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 20:00:36.000000 types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:54.125010 types-aiobotocore-ssm-sap-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-01-18 01:21:54.125010 types-aiobotocore-ssm-sap-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:54.125010 types-aiobotocore-ssm-sap-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:54.121010 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-01-18 01:18:27.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-01-18 01:18:27.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-01-18 01:18:27.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17396 2024-01-18 01:18:27.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17396 2024-01-18 01:18:27.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:26.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:54.121010 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-01-18 01:21:54.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:21:54.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:54.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:54.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:54.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:54.000000 types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/LICENSE` & `types-aiobotocore-ssm-sap-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ssm-sap-2.9.0/PKG-INFO` & `types-aiobotocore-ssm-sap-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-sap
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SsmSap 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SsmSap 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/
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
 
 <a id="types-aiobotocore-ssm-sap"></a>
 
 # types-aiobotocore-ssm-sap
 
 [![PyPI - types-aiobotocore-ssm-sap](https://img.shields.io/pypi/v/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-sap)](https://pepy.tech/project/types-aiobotocore-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SsmSap 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[aiobotocore.SsmSap 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [types-aiobotocore-ssm-sap docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/README.md` & `types-aiobotocore-ssm-sap-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-sap)](https://pepy.tech/project/types-aiobotocore-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SsmSap 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[aiobotocore.SsmSap 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [types-aiobotocore-ssm-sap docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/setup.py` & `types-aiobotocore-ssm-sap-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-sap",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SsmSap 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SsmSap 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ssm-sap type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ssm_sap": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/__init__.py` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListComponentsPaginator,
     ListDatabasesPaginator,
     ListOperationsPaginator,
 )
 
 Client = SsmSapClient
 
-
 __all__ = (
     "Client",
     "ListApplicationsPaginator",
     "ListComponentsPaginator",
     "ListDatabasesPaginator",
     "ListOperationsPaginator",
     "SsmSapClient",
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/__init__.pyi` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/__main__.py` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SsmSap 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SsmSap 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
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

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/client.py` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SsmSapClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -109,15 +108,15 @@
         """
 
     async def delete_resource_permission(
         self,
         *,
         ResourceArn: str,
         ActionType: Literal["RESTORE"] = ...,
-        SourceResourceArn: str = ...
+        SourceResourceArn: str = ...,
     ) -> DeleteResourcePermissionOutputTypeDef:
         """
         Removes permissions associated with the target database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.delete_resource_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#delete_resource_permission)
         """
@@ -167,15 +166,15 @@
 
     async def get_database(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         DatabaseId: str = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> GetDatabaseOutputTypeDef:
         """
         Gets the SAP HANA database of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_database)
@@ -222,15 +221,15 @@
 
     async def list_databases(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatabasesOutputTypeDef:
         """
         Lists the SAP HANA databases of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_databases)
@@ -239,15 +238,15 @@
 
     async def list_operations(
         self,
         *,
         ApplicationId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListOperationsOutputTypeDef:
         """
         Lists the operations performed by AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#list_operations)
         """
@@ -280,15 +279,15 @@
         ApplicationId: str,
         ApplicationType: ApplicationTypeType,
         Instances: Sequence[str],
         SapInstanceNumber: str = ...,
         Sid: str = ...,
         Tags: Mapping[str, str] = ...,
         Credentials: Sequence[ApplicationCredentialTypeDef] = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> RegisterApplicationOutputTypeDef:
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#register_application)
         """
@@ -322,15 +321,15 @@
     async def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
         CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
         Backint: BackintConfigTypeDef = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#update_application_settings)
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/client.pyi` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         """
 
     async def delete_resource_permission(
         self,
         *,
         ResourceArn: str,
         ActionType: Literal["RESTORE"] = ...,
-        SourceResourceArn: str = ...
+        SourceResourceArn: str = ...,
     ) -> DeleteResourcePermissionOutputTypeDef:
         """
         Removes permissions associated with the target database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.delete_resource_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#delete_resource_permission)
         """
@@ -163,15 +163,15 @@
 
     async def get_database(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         DatabaseId: str = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> GetDatabaseOutputTypeDef:
         """
         Gets the SAP HANA database of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.get_database)
@@ -218,15 +218,15 @@
 
     async def list_databases(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatabasesOutputTypeDef:
         """
         Lists the SAP HANA databases of an application registered with AWS Systems
         Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_databases)
@@ -235,15 +235,15 @@
 
     async def list_operations(
         self,
         *,
         ApplicationId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        Filters: Sequence[FilterTypeDef] = ...
+        Filters: Sequence[FilterTypeDef] = ...,
     ) -> ListOperationsOutputTypeDef:
         """
         Lists the operations performed by AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.list_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#list_operations)
         """
@@ -276,15 +276,15 @@
         ApplicationId: str,
         ApplicationType: ApplicationTypeType,
         Instances: Sequence[str],
         SapInstanceNumber: str = ...,
         Sid: str = ...,
         Tags: Mapping[str, str] = ...,
         Credentials: Sequence[ApplicationCredentialTypeDef] = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> RegisterApplicationOutputTypeDef:
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#register_application)
         """
@@ -318,15 +318,15 @@
     async def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
         CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
         Backint: BackintConfigTypeDef = ...,
-        DatabaseArn: str = ...
+        DatabaseArn: str = ...,
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#update_application_settings)
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/literals.py` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/literals.py`

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
     "AllocationTypeType",
     "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
     "BackintModeType",
     "ClusterStatusType",
@@ -46,15 +45,14 @@
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AllocationTypeType = Literal["ELASTIC_IP", "OVERLAY", "UNKNOWN", "VPC_SUBNET"]
 ApplicationDiscoveryStatusType = Literal[
     "DELETING", "REFRESH_FAILED", "REGISTERING", "REGISTRATION_FAILED", "SUCCESS"
 ]
 ApplicationStatusType = Literal[
     "ACTIVATED", "DELETING", "FAILED", "REGISTERING", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/literals.pyi` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/paginator.py` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "ListApplicationsPaginator",
     "ListComponentsPaginator",
     "ListDatabasesPaginator",
     "ListOperationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -65,15 +64,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 
@@ -99,15 +98,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 
@@ -118,13 +117,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/paginator.pyi` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listapplicationspaginator)
         """
 
 class ListComponentsPaginator(AioPaginator):
@@ -94,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str = ...,
         ComponentId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listdatabasespaginator)
         """
 
 class ListOperationsPaginator(AioPaginator):
@@ -112,13 +112,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/paginators/#listoperationspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/type_defs.py` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "IpAddressMemberTypeDef",
     "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap/type_defs.pyi` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/PKG-INFO` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-sap
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SsmSap 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SsmSap 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/
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
 
 <a id="types-aiobotocore-ssm-sap"></a>
 
 # types-aiobotocore-ssm-sap
 
 [![PyPI - types-aiobotocore-ssm-sap](https://img.shields.io/pypi/v/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-sap)](https://pepy.tech/project/types-aiobotocore-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SsmSap 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[aiobotocore.SsmSap 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [types-aiobotocore-ssm-sap docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-sap-2.9.0/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-sap-2.9.1/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

