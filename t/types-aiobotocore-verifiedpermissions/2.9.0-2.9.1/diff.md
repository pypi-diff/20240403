# Comparing `tmp/types-aiobotocore-verifiedpermissions-2.9.0.tar.gz` & `tmp/types-aiobotocore-verifiedpermissions-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.9.0.tar", last modified: Wed Dec 13 20:00:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.9.1.tar", last modified: Thu Jan 18 01:22:00 2024, max compression
```

## Comparing `types-aiobotocore-verifiedpermissions-2.9.0.tar` & `types-aiobotocore-verifiedpermissions-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.369027 types-aiobotocore-verifiedpermissions-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2023-12-13 20:00:43.369027 types-aiobotocore-verifiedpermissions-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:43.369027 types-aiobotocore-verifiedpermissions-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.369027 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23743 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23739 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25523 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25522 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:32.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:43.369027 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2023-12-13 20:00:43.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-13 20:00:43.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:43.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:43.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:43.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:43.000000 types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.556981 types-aiobotocore-verifiedpermissions-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-01-18 01:22:00.556981 types-aiobotocore-verifiedpermissions-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:00.556981 types-aiobotocore-verifiedpermissions-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.556981 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23748 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25522 2024-01-18 01:19:02.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25522 2024-01-18 01:19:02.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:57.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:00.556981 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-01-18 01:22:00.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-18 01:22:00.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:00.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:00.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:00.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:00.000000 types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/LICENSE` & `types-aiobotocore-verifiedpermissions-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/PKG-INFO` & `types-aiobotocore-verifiedpermissions-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-verifiedpermissions
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.VerifiedPermissions 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.VerifiedPermissions 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/
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
 
 <a id="types-aiobotocore-verifiedpermissions"></a>
 
 # types-aiobotocore-verifiedpermissions
 
 [![PyPI - types-aiobotocore-verifiedpermissions](https://img.shields.io/pypi/v/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VerifiedPermissions 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[aiobotocore.VerifiedPermissions 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/README.md` & `types-aiobotocore-verifiedpermissions-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VerifiedPermissions 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[aiobotocore.VerifiedPermissions 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/setup.py` & `types-aiobotocore-verifiedpermissions-2.9.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-verifiedpermissions",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.VerifiedPermissions 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.VerifiedPermissions 2.9.1 service generated with"
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
     keywords="aiobotocore verifiedpermissions type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_verifiedpermissions": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/__init__.py` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListPoliciesPaginator,
     ListPolicyStoresPaginator,
     ListPolicyTemplatesPaginator,
 )
 
 Client = VerifiedPermissionsClient
 
-
 __all__ = (
     "Client",
     "ListIdentitySourcesPaginator",
     "ListPoliciesPaginator",
     "ListPolicyStoresPaginator",
     "ListPolicyTemplatesPaginator",
     "VerifiedPermissionsClient",
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/__init__.pyi` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/__main__.py` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VerifiedPermissions 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.VerifiedPermissions 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
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

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/client.py` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("VerifiedPermissionsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -110,15 +109,15 @@
         """
 
     async def batch_is_authorized(
         self,
         *,
         policyStoreId: str,
         requests: Sequence[BatchIsAuthorizedInputItemTypeDef],
-        entities: EntitiesDefinitionTypeDef = ...
+        entities: EntitiesDefinitionTypeDef = ...,
     ) -> BatchIsAuthorizedOutputTypeDef:
         """
         Makes a series of decisions about multiple authorization requests for one
         principal or
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.batch_is_authorized)
@@ -143,15 +142,15 @@
 
     async def create_identity_source(
         self,
         *,
         policyStoreId: str,
         configuration: ConfigurationTypeDef,
         clientToken: str = ...,
-        principalEntityType: str = ...
+        principalEntityType: str = ...,
     ) -> CreateIdentitySourceOutputTypeDef:
         """
         Creates a reference to an Amazon Cognito user pool as an external identity
         provider
         (IdP).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.create_identity_source)
@@ -169,15 +168,15 @@
         """
 
     async def create_policy_store(
         self,
         *,
         validationSettings: ValidationSettingsTypeDef,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreatePolicyStoreOutputTypeDef:
         """
         Creates a policy store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.create_policy_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#create_policy_store)
         """
@@ -293,15 +292,15 @@
         self,
         *,
         policyStoreId: str,
         principal: EntityIdentifierTypeDef = ...,
         action: ActionIdentifierTypeDef = ...,
         resource: EntityIdentifierTypeDef = ...,
         context: ContextDefinitionTypeDef = ...,
-        entities: EntitiesDefinitionTypeDef = ...
+        entities: EntitiesDefinitionTypeDef = ...,
     ) -> IsAuthorizedOutputTypeDef:
         """
         Makes an authorization decision about a service request described in the
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.is_authorized)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#is_authorized)
@@ -312,15 +311,15 @@
         *,
         policyStoreId: str,
         identityToken: str = ...,
         accessToken: str = ...,
         action: ActionIdentifierTypeDef = ...,
         resource: EntityIdentifierTypeDef = ...,
         context: ContextDefinitionTypeDef = ...,
-        entities: EntitiesDefinitionTypeDef = ...
+        entities: EntitiesDefinitionTypeDef = ...,
     ) -> IsAuthorizedWithTokenOutputTypeDef:
         """
         Makes an authorization decision about a service request described in the
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.is_authorized_with_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#is_authorized_with_token)
@@ -328,15 +327,15 @@
 
     async def list_identity_sources(
         self,
         *,
         policyStoreId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[IdentitySourceFilterTypeDef] = ...
+        filters: Sequence[IdentitySourceFilterTypeDef] = ...,
     ) -> ListIdentitySourcesOutputTypeDef:
         """
         Returns a paginated list of all of the identity sources defined in the
         specified policy
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.list_identity_sources)
@@ -345,15 +344,15 @@
 
     async def list_policies(
         self,
         *,
         policyStoreId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: PolicyFilterTypeDef = ...
+        filter: PolicyFilterTypeDef = ...,
     ) -> ListPoliciesOutputTypeDef:
         """
         Returns a paginated list of all policies stored in the specified policy store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.list_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#list_policies)
         """
@@ -392,15 +391,15 @@
 
     async def update_identity_source(
         self,
         *,
         policyStoreId: str,
         identitySourceId: str,
         updateConfiguration: UpdateConfigurationTypeDef,
-        principalEntityType: str = ...
+        principalEntityType: str = ...,
     ) -> UpdateIdentitySourceOutputTypeDef:
         """
         Updates the specified identity source to use a new identity provider (IdP)
         source, or to change the mapping of identities from the IdP to a different
         principal entity
         type.
 
@@ -419,15 +418,15 @@
         """
 
     async def update_policy_store(
         self,
         *,
         policyStoreId: str,
         validationSettings: ValidationSettingsTypeDef,
-        description: str = ...
+        description: str = ...,
     ) -> UpdatePolicyStoreOutputTypeDef:
         """
         Modifies the validation setting for a policy store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.update_policy_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#update_policy_store)
         """
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/client.pyi` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         """
 
     async def batch_is_authorized(
         self,
         *,
         policyStoreId: str,
         requests: Sequence[BatchIsAuthorizedInputItemTypeDef],
-        entities: EntitiesDefinitionTypeDef = ...
+        entities: EntitiesDefinitionTypeDef = ...,
     ) -> BatchIsAuthorizedOutputTypeDef:
         """
         Makes a series of decisions about multiple authorization requests for one
         principal or
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.batch_is_authorized)
@@ -139,15 +139,15 @@
 
     async def create_identity_source(
         self,
         *,
         policyStoreId: str,
         configuration: ConfigurationTypeDef,
         clientToken: str = ...,
-        principalEntityType: str = ...
+        principalEntityType: str = ...,
     ) -> CreateIdentitySourceOutputTypeDef:
         """
         Creates a reference to an Amazon Cognito user pool as an external identity
         provider
         (IdP).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.create_identity_source)
@@ -165,15 +165,15 @@
         """
 
     async def create_policy_store(
         self,
         *,
         validationSettings: ValidationSettingsTypeDef,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreatePolicyStoreOutputTypeDef:
         """
         Creates a policy store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.create_policy_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#create_policy_store)
         """
@@ -289,15 +289,15 @@
         self,
         *,
         policyStoreId: str,
         principal: EntityIdentifierTypeDef = ...,
         action: ActionIdentifierTypeDef = ...,
         resource: EntityIdentifierTypeDef = ...,
         context: ContextDefinitionTypeDef = ...,
-        entities: EntitiesDefinitionTypeDef = ...
+        entities: EntitiesDefinitionTypeDef = ...,
     ) -> IsAuthorizedOutputTypeDef:
         """
         Makes an authorization decision about a service request described in the
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.is_authorized)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#is_authorized)
@@ -308,15 +308,15 @@
         *,
         policyStoreId: str,
         identityToken: str = ...,
         accessToken: str = ...,
         action: ActionIdentifierTypeDef = ...,
         resource: EntityIdentifierTypeDef = ...,
         context: ContextDefinitionTypeDef = ...,
-        entities: EntitiesDefinitionTypeDef = ...
+        entities: EntitiesDefinitionTypeDef = ...,
     ) -> IsAuthorizedWithTokenOutputTypeDef:
         """
         Makes an authorization decision about a service request described in the
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.is_authorized_with_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#is_authorized_with_token)
@@ -324,15 +324,15 @@
 
     async def list_identity_sources(
         self,
         *,
         policyStoreId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filters: Sequence[IdentitySourceFilterTypeDef] = ...
+        filters: Sequence[IdentitySourceFilterTypeDef] = ...,
     ) -> ListIdentitySourcesOutputTypeDef:
         """
         Returns a paginated list of all of the identity sources defined in the
         specified policy
         store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.list_identity_sources)
@@ -341,15 +341,15 @@
 
     async def list_policies(
         self,
         *,
         policyStoreId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: PolicyFilterTypeDef = ...
+        filter: PolicyFilterTypeDef = ...,
     ) -> ListPoliciesOutputTypeDef:
         """
         Returns a paginated list of all policies stored in the specified policy store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.list_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#list_policies)
         """
@@ -388,15 +388,15 @@
 
     async def update_identity_source(
         self,
         *,
         policyStoreId: str,
         identitySourceId: str,
         updateConfiguration: UpdateConfigurationTypeDef,
-        principalEntityType: str = ...
+        principalEntityType: str = ...,
     ) -> UpdateIdentitySourceOutputTypeDef:
         """
         Updates the specified identity source to use a new identity provider (IdP)
         source, or to change the mapping of identities from the IdP to a different
         principal entity
         type.
 
@@ -415,15 +415,15 @@
         """
 
     async def update_policy_store(
         self,
         *,
         policyStoreId: str,
         validationSettings: ValidationSettingsTypeDef,
-        description: str = ...
+        description: str = ...,
     ) -> UpdatePolicyStoreOutputTypeDef:
         """
         Modifies the validation setting for a policy store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client.update_policy_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/client/#update_policy_store)
         """
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/literals.py` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/literals.py`

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
     "DecisionType",
     "ListIdentitySourcesPaginatorName",
     "ListPoliciesPaginatorName",
     "ListPolicyStoresPaginatorName",
     "ListPolicyTemplatesPaginatorName",
     "OpenIdIssuerType",
@@ -32,15 +31,14 @@
     "VerifiedPermissionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DecisionType = Literal["ALLOW", "DENY"]
 ListIdentitySourcesPaginatorName = Literal["list_identity_sources"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListPolicyStoresPaginatorName = Literal["list_policy_stores"]
 ListPolicyTemplatesPaginatorName = Literal["list_policy_templates"]
 OpenIdIssuerType = Literal["COGNITO"]
 PolicyTypeType = Literal["STATIC", "TEMPLATE_LINKED"]
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/literals.pyi` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/paginator.py` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,78 +45,72 @@
 __all__ = (
     "ListIdentitySourcesPaginator",
     "ListPoliciesPaginator",
     "ListPolicyStoresPaginator",
     "ListPolicyTemplatesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListIdentitySourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listidentitysourcespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
-
 class ListPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
-
 class ListPolicyStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
-
 class ListPolicyTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/paginator.pyi` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,70 +47,75 @@
     "ListPoliciesPaginator",
     "ListPolicyStoresPaginator",
     "ListPolicyTemplatesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListIdentitySourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listidentitysourcespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
+
 class ListPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
+
 class ListPolicyStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
+
 class ListPolicyTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/type_defs.py` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "ContextDefinitionTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions/type_defs.pyi` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-verifiedpermissions
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.VerifiedPermissions 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.VerifiedPermissions 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/
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
 
 <a id="types-aiobotocore-verifiedpermissions"></a>
 
 # types-aiobotocore-verifiedpermissions
 
 [![PyPI - types-aiobotocore-verifiedpermissions](https://img.shields.io/pypi/v/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VerifiedPermissions 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[aiobotocore.VerifiedPermissions 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-verifiedpermissions-2.9.0/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt` & `types-aiobotocore-verifiedpermissions-2.9.1/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

