# Comparing `tmp/types-aiobotocore-license-manager-user-subscriptions-2.9.0.tar.gz` & `tmp/types-aiobotocore-license-manager-user-subscriptions-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-user-subscriptions-2.9.0.tar", last modified: Wed Dec 13 19:59:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-user-subscriptions-2.9.1.tar", last modified: Thu Jan 18 01:21:08 2024, max compression
```

## Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0.tar` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:45.941524 types-aiobotocore-license-manager-user-subscriptions-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2023-12-13 19:59:45.941524 types-aiobotocore-license-manager-user-subscriptions-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:45.941524 types-aiobotocore-license-manager-user-subscriptions-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:45.941524 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15982 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9469 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2023-12-13 19:49:13.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:12.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:45.941524 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:45.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.425217 types-aiobotocore-license-manager-user-subscriptions-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-01-18 01:21:08.425217 types-aiobotocore-license-manager-user-subscriptions-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:08.425217 types-aiobotocore-license-manager-user-subscriptions-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.421217 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15993 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:00.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:08.425217 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:08.000000 types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/LICENSE` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/PKG-INFO` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-user-subscriptions
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
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
 
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager-user-subscriptions)](https://pepy.tech/project/types-aiobotocore-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManagerUserSubscriptions 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[aiobotocore.LicenseManagerUserSubscriptions 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/README.md` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager-user-subscriptions)](https://pepy.tech/project/types-aiobotocore-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManagerUserSubscriptions 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[aiobotocore.LicenseManagerUserSubscriptions 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/setup.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,51 +7,50 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager-user-subscriptions",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.0 service generated"
-        " with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.1 service generated"
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
         "aiobotocore license-manager-user-subscriptions type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_license_manager_user_subscriptions": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/__init__.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListInstancesPaginator,
     ListProductSubscriptionsPaginator,
     ListUserAssociationsPaginator,
 )
 
 Client = LicenseManagerUserSubscriptionsClient
 
-
 __all__ = (
     "Client",
     "LicenseManagerUserSubscriptionsClient",
     "ListIdentityProvidersPaginator",
     "ListInstancesPaginator",
     "ListProductSubscriptionsPaginator",
     "ListUserAssociationsPaginator",
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/__main__.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/client.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LicenseManagerUserSubscriptionsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -92,15 +91,15 @@
 
     async def associate_user(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> AssociateUserResponseTypeDef:
         """
         Associates the user to an EC2 instance to utilize user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.associate_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#associate_user)
         """
@@ -133,15 +132,15 @@
 
     async def disassociate_user(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> DisassociateUserResponseTypeDef:
         """
         Disassociates the user from an EC2 instance providing user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.disassociate_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#disassociate_user)
         """
@@ -183,15 +182,15 @@
     async def list_product_subscriptions(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListProductSubscriptionsResponseTypeDef:
         """
         Lists the user-based subscription products available from an identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.list_product_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#list_product_subscriptions)
         """
@@ -199,73 +198,73 @@
     async def list_user_associations(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListUserAssociationsResponseTypeDef:
         """
         Lists user associations for an identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.list_user_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#list_user_associations)
         """
 
     async def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsTypeDef = ...
+        Settings: SettingsTypeDef = ...,
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#register_identity_provider)
         """
 
     async def start_product_subscription(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> StartProductSubscriptionResponseTypeDef:
         """
         Starts a product subscription for a user with the specified identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.start_product_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#start_product_subscription)
         """
 
     async def stop_product_subscription(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> StopProductSubscriptionResponseTypeDef:
         """
         Stops a product subscription for a user with the specified identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.stop_product_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#stop_product_subscription)
         """
 
     async def update_identity_provider_settings(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        UpdateSettings: UpdateSettingsTypeDef
+        UpdateSettings: UpdateSettingsTypeDef,
     ) -> UpdateIdentityProviderSettingsResponseTypeDef:
         """
         Updates additional product configuration settings for the registered identity
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.update_identity_provider_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#update_identity_provider_settings)
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/client.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     async def associate_user(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> AssociateUserResponseTypeDef:
         """
         Associates the user to an EC2 instance to utilize user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.associate_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#associate_user)
         """
@@ -129,15 +129,15 @@
 
     async def disassociate_user(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> DisassociateUserResponseTypeDef:
         """
         Disassociates the user from an EC2 instance providing user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.disassociate_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#disassociate_user)
         """
@@ -179,15 +179,15 @@
     async def list_product_subscriptions(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListProductSubscriptionsResponseTypeDef:
         """
         Lists the user-based subscription products available from an identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.list_product_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#list_product_subscriptions)
         """
@@ -195,73 +195,73 @@
     async def list_user_associations(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListUserAssociationsResponseTypeDef:
         """
         Lists user associations for an identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.list_user_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#list_user_associations)
         """
 
     async def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsTypeDef = ...
+        Settings: SettingsTypeDef = ...,
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#register_identity_provider)
         """
 
     async def start_product_subscription(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> StartProductSubscriptionResponseTypeDef:
         """
         Starts a product subscription for a user with the specified identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.start_product_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#start_product_subscription)
         """
 
     async def stop_product_subscription(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Username: str,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> StopProductSubscriptionResponseTypeDef:
         """
         Stops a product subscription for a user with the specified identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.stop_product_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#stop_product_subscription)
         """
 
     async def update_identity_provider_settings(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        UpdateSettings: UpdateSettingsTypeDef
+        UpdateSettings: UpdateSettingsTypeDef,
     ) -> UpdateIdentityProviderSettingsResponseTypeDef:
         """
         Updates additional product configuration settings for the registered identity
         provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.update_identity_provider_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#update_identity_provider_settings)
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/literals.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListIdentityProvidersPaginatorName",
     "ListInstancesPaginatorName",
     "ListProductSubscriptionsPaginatorName",
     "ListUserAssociationsPaginatorName",
     "LicenseManagerUserSubscriptionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListIdentityProvidersPaginatorName = Literal["list_identity_providers"]
 ListInstancesPaginatorName = Literal["list_instances"]
 ListProductSubscriptionsPaginatorName = Literal["list_product_subscriptions"]
 ListUserAssociationsPaginatorName = Literal["list_user_associations"]
 LicenseManagerUserSubscriptionsServiceName = Literal["license-manager-user-subscriptions"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/literals.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/paginator.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 __all__ = (
     "ListIdentityProvidersPaginator",
     "ListInstancesPaginator",
     "ListProductSubscriptionsPaginator",
     "ListUserAssociationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -81,15 +80,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
 
@@ -101,15 +100,15 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
 
@@ -121,13 +120,13 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
 class ListProductSubscriptionsPaginator(AioPaginator):
@@ -96,15 +96,15 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
 class ListUserAssociationsPaginator(AioPaginator):
@@ -115,13 +115,13 @@
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/type_defs.py` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
     "ResponseMetadataTypeDef",
     "FilterTypeDef",
     "SettingsTypeDef",
     "InstanceSummaryTypeDef",
     "PaginatorConfigTypeDef",
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-user-subscriptions
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
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
 
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager-user-subscriptions)](https://pepy.tech/project/types-aiobotocore-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManagerUserSubscriptions 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[aiobotocore.LicenseManagerUserSubscriptions 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.9.0/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-user-subscriptions-2.9.1/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

