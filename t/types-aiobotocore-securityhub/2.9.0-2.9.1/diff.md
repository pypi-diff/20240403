# Comparing `tmp/types-aiobotocore-securityhub-2.9.0.tar.gz` & `tmp/types-aiobotocore-securityhub-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-securityhub-2.9.0.tar", last modified: Wed Dec 13 20:00:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-securityhub-2.9.1.tar", last modified: Thu Jan 18 01:21:46 2024, max compression
```

## Comparing `types-aiobotocore-securityhub-2.9.0.tar` & `types-aiobotocore-securityhub-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:28.317156 types-aiobotocore-securityhub-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15996 2023-12-13 20:00:28.317156 types-aiobotocore-securityhub-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14417 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:28.317156 types-aiobotocore-securityhub-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:28.317156 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64758 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    64754 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15968 2023-12-13 19:56:00.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15966 2023-12-13 19:56:00.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21758 2023-12-13 19:56:00.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21739 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   475740 2023-12-13 19:56:14.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   475739 2023-12-13 19:56:07.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:59.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:28.317156 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15996 2023-12-13 20:00:28.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 20:00:28.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:28.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:28.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:28.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 20:00:28.000000 types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:46.929043 types-aiobotocore-securityhub-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-01-18 01:21:46.929043 types-aiobotocore-securityhub-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:46.929043 types-aiobotocore-securityhub-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:46.925043 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64775 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64772 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-01-18 01:17:32.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-01-18 01:17:32.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-01-18 01:17:32.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-01-18 01:17:32.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   475739 2024-01-18 01:17:43.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   475739 2024-01-18 01:17:41.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:31.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:46.925043 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-01-18 01:21:46.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:21:46.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:46.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:46.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:46.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:46.000000 types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-securityhub-2.9.0/LICENSE` & `types-aiobotocore-securityhub-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-securityhub-2.9.0/PKG-INFO` & `types-aiobotocore-securityhub-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securityhub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SecurityHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SecurityHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/
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
 
 <a id="types-aiobotocore-securityhub"></a>
 
 # types-aiobotocore-securityhub
 
 [![PyPI - types-aiobotocore-securityhub](https://img.shields.io/pypi/v/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securityhub)](https://pepy.tech/project/types-aiobotocore-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[aiobotocore.SecurityHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [types-aiobotocore-securityhub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-securityhub-2.9.0/README.md` & `types-aiobotocore-securityhub-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securityhub)](https://pepy.tech/project/types-aiobotocore-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[aiobotocore.SecurityHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [types-aiobotocore-securityhub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-securityhub-2.9.0/setup.py` & `types-aiobotocore-securityhub-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-securityhub",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SecurityHub 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SecurityHub 2.9.1 service generated with"
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
     keywords="aiobotocore securityhub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_securityhub": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/__init__.py` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 
 Client = SecurityHubClient
 
-
 __all__ = (
     "Client",
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsControlsPaginator",
     "DescribeStandardsPaginator",
     "GetEnabledStandardsPaginator",
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/__init__.pyi` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/__main__.py` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecurityHub 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SecurityHub 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
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

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/client.py` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SecurityHubClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -237,15 +236,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_automation_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_get_automation_rules)
         """
 
     async def batch_get_configuration_policy_associations(
         self,
         *,
-        ConfigurationPolicyAssociationIdentifiers: Sequence[ConfigurationPolicyAssociationTypeDef]
+        ConfigurationPolicyAssociationIdentifiers: Sequence[ConfigurationPolicyAssociationTypeDef],
     ) -> BatchGetConfigurationPolicyAssociationsResponseTypeDef:
         """
         Returns associations between an Security Hub configuration and a batch of
         target accounts, organizational units, or the
         root.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_configuration_policy_associations)
@@ -285,15 +284,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_import_findings)
         """
 
     async def batch_update_automation_rules(
         self,
         *,
-        UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef]
+        UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef],
     ) -> BatchUpdateAutomationRulesResponseTypeDef:
         """
         Updates one or more automation rules based on rule Amazon Resource Names (ARNs)
         and input
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_automation_rules)
@@ -308,29 +307,29 @@
         Severity: SeverityUpdateTypeDef = ...,
         VerificationState: VerificationStateType = ...,
         Confidence: int = ...,
         Criticality: int = ...,
         Types: Sequence[str] = ...,
         UserDefinedFields: Mapping[str, str] = ...,
         Workflow: WorkflowUpdateTypeDef = ...,
-        RelatedFindings: Sequence[RelatedFindingTypeDef] = ...
+        RelatedFindings: Sequence[RelatedFindingTypeDef] = ...,
     ) -> BatchUpdateFindingsResponseTypeDef:
         """
         Used by Security Hub customers to update information about their investigation
         into a
         finding.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_update_findings)
         """
 
     async def batch_update_standards_control_associations(
         self,
         *,
-        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef]
+        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef],
     ) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:
         """
         For a batch of security controls and standards, this operation updates the
         enablement status of a control in a
         standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)
@@ -369,30 +368,30 @@
         RuleOrder: int,
         RuleName: str,
         Description: str,
         Criteria: AutomationRulesFindingFiltersTypeDef,
         Actions: Sequence[AutomationRulesActionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
-        IsTerminal: bool = ...
+        IsTerminal: bool = ...,
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_automation_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_automation_rule)
         """
 
     async def create_configuration_policy(
         self,
         *,
         Name: str,
         ConfigurationPolicy: PolicyTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateConfigurationPolicyResponseTypeDef:
         """
         Creates a configuration policy with the defined configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_configuration_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_configuration_policy)
         """
@@ -627,15 +626,15 @@
         """
 
     async def enable_security_hub(
         self,
         *,
         Tags: Mapping[str, str] = ...,
         EnableDefaultStandards: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        ControlFindingGenerator: ControlFindingGeneratorType = ...,
     ) -> Dict[str, Any]:
         """
         Enables Security Hub for your account in the current Region or the Region you
         specify in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)
@@ -689,15 +688,15 @@
         """
 
     async def get_enabled_standards(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetEnabledStandardsResponseTypeDef:
         """
         Returns a list of the standards that are currently enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_enabled_standards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_enabled_standards)
         """
@@ -715,30 +714,30 @@
     async def get_finding_history(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetFindingHistoryResponseTypeDef:
         """
         Returns history for a Security Hub finding in the last 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_finding_history)
         """
 
     async def get_findings(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_findings)
         """
@@ -832,15 +831,15 @@
         """
 
     async def list_configuration_policy_associations(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: AssociationFiltersTypeDef = ...
+        Filters: AssociationFiltersTypeDef = ...,
     ) -> ListConfigurationPolicyAssociationsResponseTypeDef:
         """
         Provides information about the associations for your configuration policies and
         self-managed
         behavior.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_configuration_policy_associations)
@@ -989,15 +988,15 @@
     async def update_configuration_policy(
         self,
         *,
         Identifier: str,
         Name: str = ...,
         Description: str = ...,
         UpdatedReason: str = ...,
-        ConfigurationPolicy: PolicyTypeDef = ...
+        ConfigurationPolicy: PolicyTypeDef = ...,
     ) -> UpdateConfigurationPolicyResponseTypeDef:
         """
         Updates a configuration policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_configuration_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_configuration_policy)
         """
@@ -1013,85 +1012,85 @@
         """
 
     async def update_findings(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef,
         Note: NoteUpdateTypeDef = ...,
-        RecordState: RecordStateType = ...
+        RecordState: RecordStateType = ...,
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_findings)
         """
 
     async def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
-        GroupByAttribute: str = ...
+        GroupByAttribute: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_insight)
         """
 
     async def update_organization_configuration(
         self,
         *,
         AutoEnable: bool,
         AutoEnableStandards: AutoEnableStandardsType = ...,
-        OrganizationConfiguration: OrganizationConfigurationTypeDef = ...
+        OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of your organization in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_organization_configuration)
         """
 
     async def update_security_control(
         self,
         *,
         SecurityControlId: str,
         Parameters: Mapping[str, ParameterConfigurationTypeDef],
-        LastUpdateReason: str = ...
+        LastUpdateReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the properties of a security control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_security_control)
         """
 
     async def update_security_hub_configuration(
         self,
         *,
         AutoEnableControls: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        ControlFindingGenerator: ControlFindingGeneratorType = ...,
     ) -> Dict[str, Any]:
         """
         Updates configuration options for Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_security_hub_configuration)
         """
 
     async def update_standards_control(
         self,
         *,
         StandardsControlArn: str,
         ControlStatus: ControlStatusType = ...,
-        DisabledReason: str = ...
+        DisabledReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Used to control whether an individual security standard control is enabled or
         disabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_standards_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_standards_control)
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/client.pyi` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_automation_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_get_automation_rules)
         """
 
     async def batch_get_configuration_policy_associations(
         self,
         *,
-        ConfigurationPolicyAssociationIdentifiers: Sequence[ConfigurationPolicyAssociationTypeDef]
+        ConfigurationPolicyAssociationIdentifiers: Sequence[ConfigurationPolicyAssociationTypeDef],
     ) -> BatchGetConfigurationPolicyAssociationsResponseTypeDef:
         """
         Returns associations between an Security Hub configuration and a batch of
         target accounts, organizational units, or the
         root.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_configuration_policy_associations)
@@ -281,15 +281,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_import_findings)
         """
 
     async def batch_update_automation_rules(
         self,
         *,
-        UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef]
+        UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef],
     ) -> BatchUpdateAutomationRulesResponseTypeDef:
         """
         Updates one or more automation rules based on rule Amazon Resource Names (ARNs)
         and input
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_automation_rules)
@@ -304,29 +304,29 @@
         Severity: SeverityUpdateTypeDef = ...,
         VerificationState: VerificationStateType = ...,
         Confidence: int = ...,
         Criticality: int = ...,
         Types: Sequence[str] = ...,
         UserDefinedFields: Mapping[str, str] = ...,
         Workflow: WorkflowUpdateTypeDef = ...,
-        RelatedFindings: Sequence[RelatedFindingTypeDef] = ...
+        RelatedFindings: Sequence[RelatedFindingTypeDef] = ...,
     ) -> BatchUpdateFindingsResponseTypeDef:
         """
         Used by Security Hub customers to update information about their investigation
         into a
         finding.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_update_findings)
         """
 
     async def batch_update_standards_control_associations(
         self,
         *,
-        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef]
+        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef],
     ) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:
         """
         For a batch of security controls and standards, this operation updates the
         enablement status of a control in a
         standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)
@@ -365,30 +365,30 @@
         RuleOrder: int,
         RuleName: str,
         Description: str,
         Criteria: AutomationRulesFindingFiltersTypeDef,
         Actions: Sequence[AutomationRulesActionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
-        IsTerminal: bool = ...
+        IsTerminal: bool = ...,
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_automation_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_automation_rule)
         """
 
     async def create_configuration_policy(
         self,
         *,
         Name: str,
         ConfigurationPolicy: PolicyTypeDef,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateConfigurationPolicyResponseTypeDef:
         """
         Creates a configuration policy with the defined configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_configuration_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_configuration_policy)
         """
@@ -623,15 +623,15 @@
         """
 
     async def enable_security_hub(
         self,
         *,
         Tags: Mapping[str, str] = ...,
         EnableDefaultStandards: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        ControlFindingGenerator: ControlFindingGeneratorType = ...,
     ) -> Dict[str, Any]:
         """
         Enables Security Hub for your account in the current Region or the Region you
         specify in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)
@@ -685,15 +685,15 @@
         """
 
     async def get_enabled_standards(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetEnabledStandardsResponseTypeDef:
         """
         Returns a list of the standards that are currently enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_enabled_standards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_enabled_standards)
         """
@@ -711,30 +711,30 @@
     async def get_finding_history(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetFindingHistoryResponseTypeDef:
         """
         Returns history for a Security Hub finding in the last 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_finding_history)
         """
 
     async def get_findings(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_findings)
         """
@@ -828,15 +828,15 @@
         """
 
     async def list_configuration_policy_associations(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        Filters: AssociationFiltersTypeDef = ...
+        Filters: AssociationFiltersTypeDef = ...,
     ) -> ListConfigurationPolicyAssociationsResponseTypeDef:
         """
         Provides information about the associations for your configuration policies and
         self-managed
         behavior.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_configuration_policy_associations)
@@ -985,15 +985,15 @@
     async def update_configuration_policy(
         self,
         *,
         Identifier: str,
         Name: str = ...,
         Description: str = ...,
         UpdatedReason: str = ...,
-        ConfigurationPolicy: PolicyTypeDef = ...
+        ConfigurationPolicy: PolicyTypeDef = ...,
     ) -> UpdateConfigurationPolicyResponseTypeDef:
         """
         Updates a configuration policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_configuration_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_configuration_policy)
         """
@@ -1009,85 +1009,85 @@
         """
 
     async def update_findings(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef,
         Note: NoteUpdateTypeDef = ...,
-        RecordState: RecordStateType = ...
+        RecordState: RecordStateType = ...,
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_findings)
         """
 
     async def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
-        GroupByAttribute: str = ...
+        GroupByAttribute: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_insight)
         """
 
     async def update_organization_configuration(
         self,
         *,
         AutoEnable: bool,
         AutoEnableStandards: AutoEnableStandardsType = ...,
-        OrganizationConfiguration: OrganizationConfigurationTypeDef = ...
+        OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of your organization in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_organization_configuration)
         """
 
     async def update_security_control(
         self,
         *,
         SecurityControlId: str,
         Parameters: Mapping[str, ParameterConfigurationTypeDef],
-        LastUpdateReason: str = ...
+        LastUpdateReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the properties of a security control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_security_control)
         """
 
     async def update_security_hub_configuration(
         self,
         *,
         AutoEnableControls: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        ControlFindingGenerator: ControlFindingGeneratorType = ...,
     ) -> Dict[str, Any]:
         """
         Updates configuration options for Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_security_hub_configuration)
         """
 
     async def update_standards_control(
         self,
         *,
         StandardsControlArn: str,
         ControlStatus: ControlStatusType = ...,
-        DisabledReason: str = ...
+        DisabledReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Used to control whether an individual security standard control is enabled or
         disabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_standards_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_standards_control)
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/literals.py` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/literals.py`

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
     "AdminStatusType",
     "AssociationStatusType",
     "AssociationTypeType",
     "AutoEnableStandardsType",
     "AutomationRulesActionTypeType",
     "AwsIamAccessKeyStatusType",
@@ -83,15 +82,14 @@
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AssociationTypeType = Literal["APPLIED", "INHERITED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
 AutomationRulesActionTypeType = Literal["FINDING_FIELDS_UPDATE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/literals.pyi` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/paginator.py` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListSecurityControlDefinitionsPaginator",
     "ListStandardsControlAssociationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -121,15 +120,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
         """
 
 
@@ -184,15 +183,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
         """
 
 
@@ -204,15 +203,15 @@
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindinghistorypaginator)
         """
 
 
@@ -223,15 +222,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetFindingsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindingspaginator)
         """
 
 
@@ -271,15 +270,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listconfigurationpolicyassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: AssociationFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConfigurationPolicyAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListConfigurationPolicyAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listconfigurationpolicyassociationspaginator)
         """
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/paginator.pyi` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
         """
 
 class DescribeProductsPaginator(AioPaginator):
@@ -177,15 +177,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
         """
 
 class GetFindingHistoryPaginator(AioPaginator):
@@ -196,15 +196,15 @@
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindinghistorypaginator)
         """
 
 class GetFindingsPaginator(AioPaginator):
@@ -214,15 +214,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetFindingsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindingspaginator)
         """
 
 class GetInsightsPaginator(AioPaginator):
@@ -259,15 +259,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listconfigurationpolicyassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: AssociationFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConfigurationPolicyAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListConfigurationPolicyAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listconfigurationpolicyassociationspaginator)
         """
 
 class ListEnabledProductsForImportPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/type_defs.py` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
     "DnsRequestActionTypeDef",
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub/type_defs.pyi` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/PKG-INFO` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securityhub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SecurityHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SecurityHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/
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
 
 <a id="types-aiobotocore-securityhub"></a>
 
 # types-aiobotocore-securityhub
 
 [![PyPI - types-aiobotocore-securityhub](https://img.shields.io/pypi/v/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securityhub)](https://pepy.tech/project/types-aiobotocore-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[aiobotocore.SecurityHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [types-aiobotocore-securityhub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-securityhub-2.9.0/types_aiobotocore_securityhub.egg-info/SOURCES.txt` & `types-aiobotocore-securityhub-2.9.1/types_aiobotocore_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

