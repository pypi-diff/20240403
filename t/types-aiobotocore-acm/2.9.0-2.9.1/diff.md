# Comparing `tmp/types-aiobotocore-acm-2.9.0.tar.gz` & `tmp/types-aiobotocore-acm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-2.9.0.tar", last modified: Wed Dec 13 19:58:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-2.9.1.tar", last modified: Thu Jan 18 01:19:57 2024, max compression
```

## Comparing `types-aiobotocore-acm-2.9.0.tar` & `types-aiobotocore-acm-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.382139 types-aiobotocore-acm-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2023-12-13 19:58:29.382139 types-aiobotocore-acm-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11860 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:29.382139 types-aiobotocore-acm-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.382139 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14943 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2023-12-13 19:40:36.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2023-12-13 19:40:36.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2023-12-13 19:40:36.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-12-13 19:40:35.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.382139 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2023-12-13 19:58:29.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:58:29.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:29.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:29.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:29.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:58:29.000000 types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.937538 types-aiobotocore-acm-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-01-18 01:19:57.937538 types-aiobotocore-acm-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:57.937538 types-aiobotocore-acm-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.937538 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14942 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:34.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-18 01:02:35.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.937538 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-01-18 01:19:57.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:19:57.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:57.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:57.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:57.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:19:57.000000 types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-2.9.0/LICENSE` & `types-aiobotocore-acm-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-acm-2.9.0/PKG-INFO` & `types-aiobotocore-acm-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ACM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ACM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
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
 
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[aiobotocore.ACM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-acm-2.9.0/README.md` & `types-aiobotocore-acm-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[aiobotocore.ACM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-acm-2.9.0/setup.py` & `types-aiobotocore-acm-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ACM 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.ACM 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore acm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_acm": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/__init__.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 
 from .client import ACMClient
 from .paginator import ListCertificatesPaginator
 from .waiter import CertificateValidatedWaiter
 
 Client = ACMClient
 
-
 __all__ = ("ACMClient", "CertificateValidatedWaiter", "Client", "ListCertificatesPaginator")
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/__init__.pyi` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/__main__.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACM 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ACM 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/client.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 from .waiter import CertificateValidatedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ACMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -187,15 +186,15 @@
     async def import_certificate(
         self,
         *,
         Certificate: BlobTypeDef,
         PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
         CertificateChain: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with
         ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
@@ -206,15 +205,15 @@
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         NextToken: str = ...,
         MaxItems: int = ...,
         SortBy: Literal["CREATED_AT"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListCertificatesResponseTypeDef:
         """
         Retrieves a list of certificate ARNs and domain names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#list_certificates)
         """
@@ -264,15 +263,15 @@
         ValidationMethod: ValidationMethodType = ...,
         SubjectAlternativeNames: Sequence[str] = ...,
         IdempotencyToken: str = ...,
         DomainValidationOptions: Sequence[DomainValidationOptionTypeDef] = ...,
         Options: CertificateOptionsTypeDef = ...,
         CertificateAuthorityArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        KeyAlgorithm: KeyAlgorithmType = ...
+        KeyAlgorithm: KeyAlgorithmType = ...,
     ) -> RequestCertificateResponseTypeDef:
         """
         Requests an ACM certificate for use with other Amazon Web Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.request_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#request_certificate)
         """
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/client.pyi` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     async def import_certificate(
         self,
         *,
         Certificate: BlobTypeDef,
         PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
         CertificateChain: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with
         ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
@@ -202,15 +202,15 @@
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         NextToken: str = ...,
         MaxItems: int = ...,
         SortBy: Literal["CREATED_AT"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListCertificatesResponseTypeDef:
         """
         Retrieves a list of certificate ARNs and domain names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#list_certificates)
         """
@@ -260,15 +260,15 @@
         ValidationMethod: ValidationMethodType = ...,
         SubjectAlternativeNames: Sequence[str] = ...,
         IdempotencyToken: str = ...,
         DomainValidationOptions: Sequence[DomainValidationOptionTypeDef] = ...,
         Options: CertificateOptionsTypeDef = ...,
         CertificateAuthorityArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        KeyAlgorithm: KeyAlgorithmType = ...
+        KeyAlgorithm: KeyAlgorithmType = ...,
     ) -> RequestCertificateResponseTypeDef:
         """
         Requests an ACM certificate for use with other Amazon Web Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.request_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/client/#request_certificate)
         """
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/literals.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/literals.py`

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
     "CertificateStatusType",
     "CertificateTransparencyLoggingPreferenceType",
     "CertificateTypeType",
     "CertificateValidatedWaiterName",
     "DomainStatusType",
     "ExtendedKeyUsageNameType",
@@ -42,15 +41,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 CertificateStatusType = Literal[
     "EXPIRED",
     "FAILED",
     "INACTIVE",
     "ISSUED",
     "PENDING_VALIDATION",
     "REVOKED",
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/literals.pyi` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/paginator.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 from .type_defs import FiltersTypeDef, ListCertificatesResponseTypeDef, PaginatorConfigTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ListCertificatesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -58,13 +56,13 @@
     def paginate(
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         SortBy: Literal["CREATED_AT"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/paginators/#listcertificatespaginator)
         """
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/paginator.pyi` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -54,13 +54,13 @@
     def paginate(
         self,
         *,
         CertificateStatuses: Sequence[CertificateStatusType] = ...,
         Includes: FiltersTypeDef = ...,
         SortBy: Literal["CREATED_AT"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/paginators/#listcertificatespaginator)
         """
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/type_defs.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/type_defs.py`

 * *Files 1% similar despite different names*

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
     "TagTypeDef",
     "BlobTypeDef",
     "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
     "CertificateSummaryTypeDef",
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/type_defs.pyi` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/waiter.py` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm/waiter.pyi` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/PKG-INFO` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ACM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ACM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
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
 
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[aiobotocore.ACM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-acm-2.9.0/types_aiobotocore_acm.egg-info/SOURCES.txt` & `types-aiobotocore-acm-2.9.1/types_aiobotocore_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

