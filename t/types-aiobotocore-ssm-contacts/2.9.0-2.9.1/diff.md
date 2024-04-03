# Comparing `tmp/types-aiobotocore-ssm-contacts-2.9.0.tar.gz` & `tmp/types-aiobotocore-ssm-contacts-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-contacts-2.9.0.tar", last modified: Wed Dec 13 20:00:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-contacts-2.9.1.tar", last modified: Thu Jan 18 01:21:53 2024, max compression
```

## Comparing `types-aiobotocore-ssm-contacts-2.9.0.tar` & `types-aiobotocore-ssm-contacts-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.125098 types-aiobotocore-ssm-contacts-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2023-12-13 20:00:35.125098 types-aiobotocore-ssm-contacts-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13251 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:35.125098 types-aiobotocore-ssm-contacts-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.125098 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34361 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34357 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14393 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28622 2023-12-13 19:56:55.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28621 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:54.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:35.125098 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14833 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 20:00:35.000000 types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.065015 types-aiobotocore-ssm-contacts-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-01-18 01:21:53.065015 types-aiobotocore-ssm-contacts-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:53.065015 types-aiobotocore-ssm-contacts-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.065015 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34373 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34370 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28621 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28621 2024-01-18 01:18:25.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:24.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:53.065015 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:53.000000 types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/LICENSE` & `types-aiobotocore-ssm-contacts-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/PKG-INFO` & `types-aiobotocore-ssm-contacts-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-contacts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSMContacts 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSMContacts 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/
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
 
 <a id="types-aiobotocore-ssm-contacts"></a>
 
 # types-aiobotocore-ssm-contacts
 
 [![PyPI - types-aiobotocore-ssm-contacts](https://img.shields.io/pypi/v/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMContacts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[aiobotocore.SSMContacts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [types-aiobotocore-ssm-contacts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/README.md` & `types-aiobotocore-ssm-contacts-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMContacts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[aiobotocore.SSMContacts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [types-aiobotocore-ssm-contacts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/setup.py` & `types-aiobotocore-ssm-contacts-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-contacts",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSMContacts 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SSMContacts 2.9.1 service generated with"
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
     keywords="aiobotocore ssm-contacts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ssm_contacts": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/__init__.py` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     ListRotationOverridesPaginator,
     ListRotationShiftsPaginator,
     ListRotationsPaginator,
 )
 
 Client = SSMContactsClient
 
-
 __all__ = (
     "Client",
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
     "ListEngagementsPaginator",
     "ListPageReceiptsPaginator",
     "ListPageResolutionsPaginator",
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/__init__.pyi` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/__main__.py` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMContacts 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SSMContacts 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/client.py` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMContactsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -119,15 +118,15 @@
         self,
         *,
         PageId: str,
         AcceptType: AcceptTypeType,
         AcceptCode: str,
         ContactChannelId: str = ...,
         Note: str = ...,
-        AcceptCodeValidation: AcceptCodeValidationType = ...
+        AcceptCodeValidation: AcceptCodeValidationType = ...,
     ) -> Dict[str, Any]:
         """
         Used to acknowledge an engagement to a contact channel during an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.accept_page)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#accept_page)
         """
@@ -162,15 +161,15 @@
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
         Plan: PlanTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
         in phases during an
         incident.
 
@@ -182,15 +181,15 @@
         self,
         *,
         ContactId: str,
         Name: str,
         Type: ChannelTypeType,
         DeliveryAddress: ContactChannelAddressTypeDef,
         DeferActivation: bool = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateContactChannelResultTypeDef:
         """
         A contact channel is the method that Incident Manager uses to engage your
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_contact_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_contact_channel)
@@ -201,15 +200,15 @@
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation)
         """
@@ -217,15 +216,15 @@
     async def create_rotation_override(
         self,
         *,
         RotationId: str,
         NewContactIds: Sequence[str],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateRotationOverrideResultTypeDef:
         """
         Creates an override for a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation_override)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation_override)
         """
@@ -363,30 +362,30 @@
 
     async def list_contacts(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         AliasPrefix: str = ...,
-        Type: ContactTypeType = ...
+        Type: ContactTypeType = ...,
     ) -> ListContactsResultTypeDef:
         """
         Lists all contacts and escalation plans in Incident Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_contacts)
         """
 
     async def list_engagements(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncidentId: str = ...,
-        TimeRangeValue: TimeRangeTypeDef = ...
+        TimeRangeValue: TimeRangeTypeDef = ...,
     ) -> ListEngagementsResultTypeDef:
         """
         Lists all engagements that have happened in an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_engagements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_engagements)
         """
@@ -438,15 +437,15 @@
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
         Returns a list of shifts based on rotation configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_preview_rotation_shifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_preview_rotation_shifts)
         """
@@ -454,15 +453,15 @@
     async def list_rotation_overrides(
         self,
         *,
         RotationId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRotationOverridesResultTypeDef:
         """
         Retrieves a list of overrides currently specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_overrides)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_rotation_overrides)
         """
@@ -470,15 +469,15 @@
     async def list_rotation_shifts(
         self,
         *,
         RotationId: str,
         EndTime: TimestampTypeDef,
         StartTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRotationShiftsResultTypeDef:
         """
         Returns a list of shifts generated by an existing rotation in the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_shifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_rotation_shifts)
         """
@@ -523,15 +522,15 @@
         ContactId: str,
         Sender: str,
         Subject: str,
         Content: str,
         PublicSubject: str = ...,
         PublicContent: str = ...,
         IncidentId: str = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> StartEngagementResultTypeDef:
         """
         Starts an engagement to a contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.start_engagement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#start_engagement)
         """
@@ -573,15 +572,15 @@
         """
 
     async def update_contact_channel(
         self,
         *,
         ContactChannelId: str,
         Name: str = ...,
-        DeliveryAddress: ContactChannelAddressTypeDef = ...
+        DeliveryAddress: ContactChannelAddressTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a contact's contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact_channel)
         """
@@ -589,15 +588,15 @@
     async def update_rotation(
         self,
         *,
         RotationId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         ContactIds: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
-        TimeZoneId: str = ...
+        TimeZoneId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_rotation)
         """
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/client.pyi` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         self,
         *,
         PageId: str,
         AcceptType: AcceptTypeType,
         AcceptCode: str,
         ContactChannelId: str = ...,
         Note: str = ...,
-        AcceptCodeValidation: AcceptCodeValidationType = ...
+        AcceptCodeValidation: AcceptCodeValidationType = ...,
     ) -> Dict[str, Any]:
         """
         Used to acknowledge an engagement to a contact channel during an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.accept_page)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#accept_page)
         """
@@ -158,15 +158,15 @@
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
         Plan: PlanTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
         in phases during an
         incident.
 
@@ -178,15 +178,15 @@
         self,
         *,
         ContactId: str,
         Name: str,
         Type: ChannelTypeType,
         DeliveryAddress: ContactChannelAddressTypeDef,
         DeferActivation: bool = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateContactChannelResultTypeDef:
         """
         A contact channel is the method that Incident Manager uses to engage your
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_contact_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_contact_channel)
@@ -197,15 +197,15 @@
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation)
         """
@@ -213,15 +213,15 @@
     async def create_rotation_override(
         self,
         *,
         RotationId: str,
         NewContactIds: Sequence[str],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> CreateRotationOverrideResultTypeDef:
         """
         Creates an override for a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation_override)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation_override)
         """
@@ -359,30 +359,30 @@
 
     async def list_contacts(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         AliasPrefix: str = ...,
-        Type: ContactTypeType = ...
+        Type: ContactTypeType = ...,
     ) -> ListContactsResultTypeDef:
         """
         Lists all contacts and escalation plans in Incident Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_contacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_contacts)
         """
 
     async def list_engagements(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncidentId: str = ...,
-        TimeRangeValue: TimeRangeTypeDef = ...
+        TimeRangeValue: TimeRangeTypeDef = ...,
     ) -> ListEngagementsResultTypeDef:
         """
         Lists all engagements that have happened in an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_engagements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_engagements)
         """
@@ -434,15 +434,15 @@
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
         Returns a list of shifts based on rotation configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_preview_rotation_shifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_preview_rotation_shifts)
         """
@@ -450,15 +450,15 @@
     async def list_rotation_overrides(
         self,
         *,
         RotationId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRotationOverridesResultTypeDef:
         """
         Retrieves a list of overrides currently specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_overrides)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_rotation_overrides)
         """
@@ -466,15 +466,15 @@
     async def list_rotation_shifts(
         self,
         *,
         RotationId: str,
         EndTime: TimestampTypeDef,
         StartTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRotationShiftsResultTypeDef:
         """
         Returns a list of shifts generated by an existing rotation in the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_shifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_rotation_shifts)
         """
@@ -519,15 +519,15 @@
         ContactId: str,
         Sender: str,
         Subject: str,
         Content: str,
         PublicSubject: str = ...,
         PublicContent: str = ...,
         IncidentId: str = ...,
-        IdempotencyToken: str = ...
+        IdempotencyToken: str = ...,
     ) -> StartEngagementResultTypeDef:
         """
         Starts an engagement to a contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.start_engagement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#start_engagement)
         """
@@ -569,15 +569,15 @@
         """
 
     async def update_contact_channel(
         self,
         *,
         ContactChannelId: str,
         Name: str = ...,
-        DeliveryAddress: ContactChannelAddressTypeDef = ...
+        DeliveryAddress: ContactChannelAddressTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a contact's contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact_channel)
         """
@@ -585,15 +585,15 @@
     async def update_rotation(
         self,
         *,
         RotationId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         ContactIds: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
-        TimeZoneId: str = ...
+        TimeZoneId: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_rotation)
         """
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/literals.py` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/literals.py`

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
     "AcceptCodeValidationType",
     "AcceptTypeType",
     "ActivationStatusType",
     "ChannelTypeType",
     "ContactTypeType",
     "DayOfWeekType",
@@ -43,15 +42,14 @@
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
 ContactTypeType = Literal["ESCALATION", "ONCALL_SCHEDULE", "PERSONAL"]
 DayOfWeekType = Literal["FRI", "MON", "SAT", "SUN", "THU", "TUE", "WED"]
 ListContactChannelsPaginatorName = Literal["list_contact_channels"]
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/literals.pyi` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/paginator.py` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -113,15 +112,15 @@
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactspaginator)
         """
 
 
@@ -132,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listengagementspaginator)
         """
 
 
@@ -216,15 +215,15 @@
         EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
 
@@ -236,15 +235,15 @@
 
     def paginate(
         self,
         *,
         RotationId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
 
@@ -256,15 +255,15 @@
 
     def paginate(
         self,
         *,
         RotationId: str,
         EndTime: TimestampTypeDef,
         StartTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/paginator.pyi` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactspaginator)
         """
 
 class ListEngagementsPaginator(AioPaginator):
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listengagementspaginator)
         """
 
 class ListPageReceiptsPaginator(AioPaginator):
@@ -206,15 +206,15 @@
         EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
 class ListRotationOverridesPaginator(AioPaginator):
@@ -225,15 +225,15 @@
 
     def paginate(
         self,
         *,
         RotationId: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
 class ListRotationShiftsPaginator(AioPaginator):
@@ -244,15 +244,15 @@
 
     def paginate(
         self,
         *,
         RotationId: str,
         EndTime: TimestampTypeDef,
         StartTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
 class ListRotationsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/type_defs.py` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/type_defs.py`

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
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts/type_defs.pyi` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-contacts
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SSMContacts 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SSMContacts 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/
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
 
 <a id="types-aiobotocore-ssm-contacts"></a>
 
 # types-aiobotocore-ssm-contacts
 
 [![PyPI - types-aiobotocore-ssm-contacts](https://img.shields.io/pypi/v/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMContacts 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[aiobotocore.SSMContacts 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [types-aiobotocore-ssm-contacts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ssm-contacts-2.9.0/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-contacts-2.9.1/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

