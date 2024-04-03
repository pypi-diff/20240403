# Comparing `tmp/types-aiobotocore-codeguru-security-2.9.0.tar.gz` & `tmp/types-aiobotocore-codeguru-security-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-security-2.9.0.tar", last modified: Wed Dec 13 19:58:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-security-2.9.1.tar", last modified: Thu Jan 18 01:20:21 2024, max compression
```

## Comparing `types-aiobotocore-codeguru-security-2.9.0.tar` & `types-aiobotocore-codeguru-security-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.845930 types-aiobotocore-codeguru-security-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2023-12-13 19:58:54.845930 types-aiobotocore-codeguru-security-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:54.845930 types-aiobotocore-codeguru-security-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.845930 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14242 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2023-12-13 19:42:55.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2023-12-13 19:42:56.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2023-12-13 19:42:55.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:54.845930 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:58:54.000000 types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.161439 types-aiobotocore-codeguru-security-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-01-18 01:20:21.161439 types-aiobotocore-codeguru-security-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:21.161439 types-aiobotocore-codeguru-security-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.161439 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-01-18 01:04:52.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:51.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:21.161439 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-01-18 01:20:21.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:21.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:21.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:21.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:21.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:21.000000 types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/LICENSE` & `types-aiobotocore-codeguru-security-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-codeguru-security-2.9.0/PKG-INFO` & `types-aiobotocore-codeguru-security-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
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
 
 <a id="types-aiobotocore-codeguru-security"></a>
 
 # types-aiobotocore-codeguru-security
 
 [![PyPI - types-aiobotocore-codeguru-security](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruSecurity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[aiobotocore.CodeGuruSecurity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
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
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/README.md` & `types-aiobotocore-codeguru-security-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruSecurity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[aiobotocore.CodeGuruSecurity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
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
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/setup.py` & `types-aiobotocore-codeguru-security-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-security",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeGuruSecurity 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CodeGuruSecurity 2.9.1 service generated with"
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
     keywords="aiobotocore codeguru-security type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeguru_security": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/__init__.py` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import CodeGuruSecurityClient
 from .paginator import GetFindingsPaginator, ListFindingsMetricsPaginator, ListScansPaginator
 
 Client = CodeGuruSecurityClient
 
-
 __all__ = (
     "Client",
     "CodeGuruSecurityClient",
     "GetFindingsPaginator",
     "ListFindingsMetricsPaginator",
     "ListScansPaginator",
 )
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/__init__.pyi` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/__main__.py` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruSecurity 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruSecurity 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
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

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/client.py` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeGuruSecurityClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -115,15 +114,15 @@
         self,
         *,
         resourceId: ResourceIdTypeDef,
         scanName: str,
         analysisType: AnalysisTypeType = ...,
         clientToken: str = ...,
         scanType: ScanTypeType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateScanResponseTypeDef:
         """
         Use to create a scan using code uploaded to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.create_scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#create_scan)
         """
@@ -160,15 +159,15 @@
 
     async def get_findings(
         self,
         *,
         scanName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: StatusType = ...
+        status: StatusType = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#get_findings)
         """
@@ -196,15 +195,15 @@
 
     async def list_findings_metrics(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#list_findings_metrics)
         """
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/client.pyi` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         self,
         *,
         resourceId: ResourceIdTypeDef,
         scanName: str,
         analysisType: AnalysisTypeType = ...,
         clientToken: str = ...,
         scanType: ScanTypeType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateScanResponseTypeDef:
         """
         Use to create a scan using code uploaded to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.create_scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#create_scan)
         """
@@ -156,15 +156,15 @@
 
     async def get_findings(
         self,
         *,
         scanName: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: StatusType = ...
+        status: StatusType = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of all findings generated by a particular scan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.get_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#get_findings)
         """
@@ -192,15 +192,15 @@
 
     async def list_findings_metrics(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListFindingsMetricsResponseTypeDef:
         """
         Returns metrics about all findings in an account within a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#list_findings_metrics)
         """
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/literals.py` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/literals.py`

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
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -32,15 +31,14 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/literals.pyi` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/paginator.py` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     ListScansResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("GetFindingsPaginator", "ListFindingsMetricsPaginator", "ListScansPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -59,15 +58,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#getfindingspaginator)
         """
 
 
@@ -78,15 +77,15 @@
     """
 
     def paginate(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/paginator.pyi` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#getfindingspaginator)
         """
 
 class ListFindingsMetricsPaginator(AioPaginator):
@@ -74,15 +74,15 @@
     """
 
     def paginate(
         self,
         *,
         endDate: TimestampTypeDef,
         startDate: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 class ListScansPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/type_defs.py` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security/type_defs.pyi` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
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
 
 <a id="types-aiobotocore-codeguru-security"></a>
 
 # types-aiobotocore-codeguru-security
 
 [![PyPI - types-aiobotocore-codeguru-security](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruSecurity 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[aiobotocore.CodeGuruSecurity 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
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
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-codeguru-security-2.9.0/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-security-2.9.1/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

